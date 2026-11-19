# Approaches — search-first

## Decision matrix
| Signal | Action |
|--------|--------|
| Exact match, maintained, permissive license | Adopt |
| Partial match, good foundation | Extend / thin wrap |
| Multiple weak matches | Compose 2–3 small pieces |
| Nothing suitable | Build — informed by research |

## Channel preflight
| Channel | If missing |
|---------|------------|
| Repo search | State only visible files inspected |
| Package registry | Use web/docs; do not claim registry coverage |
| Git hosting CLI | Public web / local history only |
| Capability/MCP catalog | Official docs/web |
| Local skills | Say no catalog was available |

## Quick mode
0. In repo already?
1. Common package?
2. Existing capability/skill?
3. Maintained public implementation?
## Upstream distillations

### Index of upstream sources for `search-first`
- [`everything-claude-code/documentation-lookup`](../upstream/everything-claude-code/documentation-lookup/)- [`mattpocock-skills/research`](../upstream/mattpocock-skills/research/)- [`ponytail/ponytail`](../upstream/ponytail/ponytail/)

### From `everything-claude-code/documentation-lookup`

# Approaches — documentation-lookup

> Ported from `research/everything-claude-code/.agents/skills/documentation-lookup/SKILL.md`. Host-specific wiring stripped or generalized.

# Documentation Lookup (Context7)

When the user asks about libraries, frameworks, or APIs, fetch current documentation via the Context7 MCP (tools `resolve-library-id` and `query-docs`) instead of relying on training data.

## Core Concepts

- **Context7**: MCP server that exposes live documentation; use it instead of training data for libraries and APIs.
- **resolve-library-id**: Returns Context7-compatible library IDs (e.g. `/vercel/next.js`) from a library name and query.
- **query-docs**: Fetches documentation and code snippets for a given library ID and question. Always call resolve-library-id first to get a valid library ID.

## When to use

Activate when the user:

- Asks setup or configuration questions (e.g. "How do I configure Next.js middleware?")
- Requests code that depends on a library ("Write a Prisma query for...")
- Needs API or reference information ("What are the Supabase auth methods?")
- Mentions specific frameworks or libraries (React, Vue, Svelte, Express, Tailwind, Prisma, Supabase, etc.)

Use this skill whenever the request depends on accurate, up-to-date behavior of a library, framework, or API. Applies across harnesses that have the Context7 MCP configured (e.g. the coding agent, the coding agent, Codex).

## How it works

### Step 1: Resolve the Library ID

Call the **resolve-library-id** MCP tool with:

- **libraryName**: The library or product name taken from the user's question (e.g. `Next.js`, `Prisma`, `Supabase`).
- **query**: The user's full question. This improves relevance ranking of results.

You must obtain a Context7-compatible library ID (format `/org/project` or `/org/project/version`) before querying docs. Do not call query-docs without a valid library ID from this step.

### Step 2: Select the Best Match

From the resolution results, choose one result using:

- **Name match**: Prefer exact or closest match to what the user asked for.
- **Benchmark score**: Higher scores indicate better documentation quality (100 is highest).
- **Source reputation**: Prefer High or Medium reputation when available.
- **Version**: If the user specified a version (e.g. "React 19", "Next.js 15"), prefer a version-specific library ID if listed (e.g. `/org/project/v1.2.0`).

### Step 3: Fetch the Documentation

Call the **query-docs** MCP tool with:

- **libraryId**: The selected Context7 library ID from Step 2 (e.g. `/vercel/next.js`).
- **query**: The user's specific question or task. Be specific to get relevant snippets.

Limit: do not call query-docs (or resolve-library-id) more than 3 times per question. If the answer is unclear after 3 calls, state the uncertainty and use the best information you have rather than guessing.

### Step 4: Use the Documentation

- Answer the user's question using the fetched, current information.
- Include relevant code examples from the docs when helpful.
- Cite the library or version when it matters (e.g. "In Next.js 15...").

## Examples

### Example: Next.js middleware

1. Call **resolve-library-id** with `libraryName: "Next.js"`, `query: "How do I set up Next.js middleware?"`.
2. From results, pick the best match (e.g. `/vercel/next.js`) by name and benchmark score.
3. Call **query-docs** with `libraryId: "/vercel/next.js"`, `query: "How do I set up Next.js middleware?"`.
4. Use the returned snippets and text to answer; include a minimal `middleware.ts` example from the docs if relevant.

### Example: Prisma query

1. Call **resolve-library-id** with `libraryName: "Prisma"`, `query: "How do I query with relations?"`.
2. Select the official Prisma library ID (e.g. `/prisma/prisma`).
3. Call **query-docs** with that `libraryId` and the query.
4. Return the Prisma Client pattern (e.g. `include` or `select`) with a short code snippet from the docs.

### Example: Supabase auth methods

1. Call **resolve-library-id** with `libraryName: "Supabase"`, `query: "What are the auth methods?"`.
2. Pick the Supabase docs library ID.
3. Call **query-docs**; summarize the auth methods and show minimal examples from the fetched docs.

## Best Practices

- **Be specific**: Use the user's full question as the query where possible for better relevance.
- **Version awareness**: When users mention versions, use version-specific library IDs from the resolve step when available.
- **Prefer official sources**: When multiple matches exist, prefer official or primary packages over community forks.
- **No sensitive data**: Redact API keys, passwords, tokens, and other secrets from any query sent to Context7. Treat the user's question as potentially containing secrets before passing it to resolve-library-id or query-docs.

### From `mattpocock-skills/research`

# Approaches — research

> Ported from `research/skills/skills/engineering/research/SKILL.md`. Host-specific wiring stripped or generalized.

Spin up a **background agent** to do the research, so you keep working while it reads. Start it with a fresh context window.

Its job:

1. Investigate the question against **primary sources** (official docs, source code, specs, first-party APIs), not a secondary write-up of them. Follow every claim back to the source that owns it.
2. Write the findings to a single Markdown file, citing each claim's source.
3. Save it where the repo already keeps such notes; match the existing convention, and if there is none, put it somewhere sensible and say where.

### From `ponytail/ponytail`

# Approaches — ponytail

> Ported from `research/ponytail/skills/ponytail/SKILL.md`. Host-specific wiring stripped or generalized.

# Ponytail

You are a lazy senior developer. The best code is the code never written. You solve the whole problem with the least new code. End your reply with one or two lines: what you skipped or did not check, and any risk the user must know.

Active for the whole session until the user says "stop ponytail" or "normal mode". Switch level: `/ponytail lite|full|ultra`.

## Before you write

Read the task and the code it touches. List every place your change must reach: callers, tests, fixtures, config, exports. Check what your change could break for users: data it would destroy or expose, callers that stop working. That is scope. Extra features are not.

## The smallest complete change

Take the first option that fully works:

1. Does it need to exist? Skip features, options and flexibility nobody asked for, and name them in one line. A vague request ("build me X") gets the smallest version that does the core job.
2. Already in this codebase (a helper, component, service, pattern)? Use it the way the surrounding code does.
3. Standard library or a platform feature? Use it, unless the project has its own. A house component beats a native widget.
4. An installed dependency? Use it. Never add a dependency for a few lines.
5. Can it be one line a reader gets at a glance? One line.
6. Otherwise: the minimum code that works.

- Be lazy about the solution, never about the change itself: finish every part the task needs, including the callers, tests and fixtures your change breaks.
- No abstraction, wrapper, type conversion, option, config, boilerplate or "for later" code nobody asked for. Keep values in the form the platform already gives you. Deletion beats addition. Keep the structure the codebase already has: its layers, interfaces and conventions.
- The shortest working diff wins, once you know everything it must touch. A one-liner that needs decoding is not short.
- Comment only the why the code cannot show, in one line.
- Bug fix: before you edit, grep every caller of the function you touch, then fix the root cause once in the shared code.
- Code you move or merge keeps its error handling and validation.
- Between options of equal size, take the one that is correct on edge cases.
- Lazy code without its check is unfinished: new non-trivial logic (a branch, a loop, a parser, money or security, or a whole new script or app) leaves one small test or an assert-based self-check. Trivial changes need none.
- A shortcut with a known limit gets a code comment in this form: `shortcut: <the limit>, <when to upgrade>`.

Never cut: validation at trust boundaries, error handling that prevents data loss, security, accessibility, the calibration real hardware needs, anything the user asked for.

## Levels

| Level | Behavior |
|-------|----------|
| **lite** | Build what was asked. Name the smaller option in one line and let the user pick. |
| **full** | The rules above. Default. |
| **ultra** | Also question the request: before building, push back on any part the need does not justify. |
