# DoT — Domain of Truth (harness-agnostic skill format)

DoT is the **portable source of truth** for agent skills. One skill pack loads into Cursor, Claude Code, Codex, OpenCode, Gemini, Copilot, AGENTS.md digests, or any future harness.

## Design goals

1. **Harness-agnostic core** — behavior lives in Markdown + YAML, not in host-specific hooks.
2. **Capability-based tools** — skills declare abstract capabilities (`browser.navigate`), not `mcp__chrome__*` names.
3. **Role = skill** — each skill is a specialist with tools, approaches, and hard rules.
4. **Adapters are thin** — host folders only map capabilities → concrete tools / install paths.
5. **Progressive disclosure** — `SKILL.md` is the always-loaded core; `approaches.md` / `rules.md` / `tools.md` load on demand.

## Directory layout

```
skills/
  _meta/
    FORMAT.md           # this file
    MANIFEST.yaml       # curated catalog
  _tools/
    CAPABILITIES.md     # abstract tool vocabulary
  <skill-id>/           # curated roles (composed workflows)
    SKILL.md
    tools.md
    approaches.md       # includes ## Upstream distillations
    rules.md
  upstream/
    <research-repo>/
      <skill-name>/     # 1:1 DoT port of a research skill
        SKILL.md
        tools.md
        approaches.md   # full agnosticized methodology
        rules.md
        source.md
        references/     # optional copied md refs
```

Regenerate ports: `python3 scripts/port_upstream_skills.py`  
Re-enrich roles: `python3 scripts/enrich_curated_from_upstream.py`

## SKILL.md frontmatter (required)

```yaml
---
id: minimal-coder                 # kebab-case, stable
name: Minimal Coder               # human title
version: 1.0.0
description: >-                   # WHAT + WHEN (third person); discovery text
  Writes the smallest complete change...
role: Lazy Senior Developer       # persona label
category: engineering             # product|engineering|design|research|security|ops|meta
triggers:                         # phrases that should activate this skill
  - be lazy
  - yagni
  - simplest solution
capabilities_required:            # from _tools/CAPABILITIES.md
  - filesystem.read
  - filesystem.edit
  - search.code
capabilities_optional:
  - shell.exec
  - ask_user
sources:                          # research provenance
  - research/ponytail
harness: any                      # always "any" for DoT cores
---
```

## Body sections (required in SKILL.md)

1. **Role** — who the agent becomes
2. **When to use** — activation conditions
3. **Workflow** — short numbered steps (detail → `approaches.md`)
4. **Done when** — exit criteria
5. **See also** — links to sibling files and related skills

## Capability model

Skills must **not** name harness-specific tools. Map at adapter time:

| Capability | Cursor example | Claude Code example | Codex example |
|------------|----------------|---------------------|---------------|
| `filesystem.read` | Read | Read | read_file |
| `browser.navigate` | browser MCP / IDE browser | chrome MCP / gstack browse | browser tool |
| `ask_user` | AskQuestion | AskUserQuestion | prompt |

Full vocabulary: [`../_tools/CAPABILITIES.md`](../_tools/CAPABILITIES.md)

## Adapter contract

Any harness adapter must:

1. Discover skills via `MANIFEST.yaml` or by scanning `*/SKILL.md`
2. Inject `description` into the host's skill index
3. On activation, load `SKILL.md` then optionally `tools.md` / `approaches.md` / `rules.md`
4. Resolve `capabilities_*` to host tools (fail soft if optional missing; refuse if required missing)
5. Never rewrite DoT rule text — only wrap it

See `docs/adapters.md` for per-host recipes (Cursor, Claude Code, Codex, AGENTS.md, generic).

## Compatibility

- Compatible with the emerging **Agent Skills** `SKILL.md` convention (name + description frontmatter).
- Extra DoT fields (`id`, `role`, `capabilities_*`, `sources`) are ignored by hosts that do not understand them.
- For rules-only hosts, concatenate `rules.md` sections into `AGENTS.md`.
