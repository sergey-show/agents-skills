# Approaches — content-writer

## Core rules
1. Lead with the concrete thing
2. Explain after the example
3. Tight sentences unless voice is expansive
4. Proof over adjectives
5. Never invent facts or customer evidence

## Structures
### Technical guides
Open with what the reader gets · code/commands/output in major sections · actionable close

### Essays
Start with tension/observation · one argument thread per section · opinions answer to evidence

### Newsletters
First screen does real work · no diary filler · section labels only if they help scan

## Banned patterns
"In today's rapidly evolving landscape" · game-changer/cutting-edge · fake vulnerability arcs · engagement-only closing questions · biography padding
## Upstream distillations

### Index of upstream sources for `content-writer`
- [`everything-claude-code/article-writing`](../upstream/everything-claude-code/article-writing/)- [`everything-claude-code/content-engine`](../upstream/everything-claude-code/content-engine/)

### From `everything-claude-code/article-writing`

# Approaches — article-writing

> Ported from `research/everything-claude-code/.agents/skills/article-writing/SKILL.md`. Host-specific wiring stripped or generalized.

# Article Writing

Write long-form content that sounds like an actual person with a point of view, not an LLM smoothing itself into paste.

## When to Activate

- drafting blog posts, essays, launch posts, guides, tutorials, or newsletter issues
- turning notes, transcripts, or research into polished articles
- matching an existing founder, operator, or brand voice from examples
- tightening structure, pacing, and evidence in already-written long-form copy

## Core Rules

1. Lead with the concrete thing: artifact, example, output, anecdote, number, screenshot, or code.
2. Explain after the example, not before.
3. Keep sentences tight unless the source voice is intentionally expansive.
4. Use proof instead of adjectives.
5. Never invent facts, credibility, or customer evidence.

## Voice Handling

If the user wants a specific voice, run `brand-voice` first and reuse its `VOICE PROFILE`.
Do not duplicate a second style-analysis pass here unless the user explicitly asks for one.

If no voice references are given, default to a sharp operator voice: concrete, unsentimental, useful.

## Banned Patterns

Delete and rewrite any of these:
- "In today's rapidly evolving landscape"
- "game-changer", "cutting-edge", "revolutionary"
- "here's why this matters" as a standalone bridge
- fake vulnerability arcs
- a closing question added only to juice engagement
- biography padding that does not move the argument
- generic AI throat-clearing that delays the point

## Writing Process

1. Clarify the audience and purpose.
2. Build a hard outline with one job per section.
3. Start sections with proof, artifact, conflict, or example.
4. Expand only where the next sentence earns space.
5. Cut anything that sounds templated, overexplained, or self-congratulatory.

## Structure Guidance

### Technical Guides

- open with what the reader gets
- use code, commands, screenshots, or concrete output in major sections
- end with actionable takeaways, not a soft recap

### Essays / Opinion

- start with tension, contradiction, or a specific observation
- keep one argument thread per section
- make opinions answer to evidence

### Newsletters

- keep the first screen doing real work
- do not front-load diary filler
- use section labels only when they improve scanability

## Quality Gate

Before delivering:
- factual claims are backed by provided sources
- generic AI transitions are gone
- the voice matches the supplied examples or the agreed `VOICE PROFILE`
- every section adds something new
- formatting matches the intended medium

### From `everything-claude-code/content-engine`

# Approaches — content-engine

> Ported from `research/everything-claude-code/.agents/skills/content-engine/SKILL.md`. Host-specific wiring stripped or generalized.

# Content Engine

Build platform-native content without flattening the author's real voice into platform slop.

## When to Activate

- writing X posts or threads
- drafting LinkedIn posts or launch updates
- scripting short-form video or YouTube explainers
- repurposing articles, podcasts, demos, docs, or internal notes into public content
- building a launch sequence or ongoing content system around a product, insight, or narrative

## Non-Negotiables

1. Start from source material, not generic post formulas.
2. Adapt the format for the platform, not the persona.
3. One post should carry one actual claim.
4. Specificity beats adjectives.
5. No engagement bait unless the user explicitly asks for it.

## Source-First Workflow

Before drafting, identify the source set:
- published articles
- notes or internal memos
- product demos
- docs or changelogs
- transcripts
- screenshots
- prior posts from the same author

If the user wants a specific voice, build a voice profile from real examples before writing.
Use `brand-voice` as the canonical workflow when voice consistency matters across more than one output.

## Voice Handling

`brand-voice` is the canonical voice layer.

Run it first when:

- there are multiple downstream outputs
- the user explicitly cares about writing style
- the content is launch, outreach, or reputation-sensitive

Reuse the resulting `VOICE PROFILE` here instead of rebuilding a second voice model.
If the user wants Affaan / ECC voice specifically, still treat `brand-voice` as the source of truth and feed it the best live or source-derived material available.

## Hard Bans

Delete and rewrite any of these:
- "In today's rapidly evolving landscape"
- "game-changer", "revolutionary", "cutting-edge"
- "here's why this matters" unless it is followed immediately by something concrete
- ending with a LinkedIn-style question just to farm replies
- forced casualness on LinkedIn
- fake engagement padding that was not present in the source material

## Platform Adaptation Rules

### X

- open with the strongest claim, artifact, or tension
- keep the compression if the source voice is compressed
- if writing a thread, each post must advance the argument
- do not pad with context the audience does not need

### LinkedIn

- expand only enough for people outside the immediate niche to follow
- do not turn it into a fake lesson post unless the source material actually is reflective
- no corporate inspiration cadence
- no praise-stacking, no "journey" filler

### Short Video

- script around the visual sequence and proof points
- first seconds should show the result, problem, or punch
- do not write narration that sounds better on paper than on screen

### YouTube

- show the result or tension early
- organize by argument or progression, not filler sections
- use chaptering only when it helps clarity

### Newsletter

- open with the point, conflict, or artifact
- do not spend the first paragraph warming up
- every section needs to add something new

## Repurposing Flow

1. Pick the anchor asset.
2. Extract 3 to 7 atomic claims or scenes.
3. Rank them by sharpness, novelty, and proof.
4. Assign one strong idea per output.
5. Adapt structure for each platform.
6. Strip platform-shaped filler.
7. Run the quality gate.

## Deliverables

When asked for a campaign, return:
- a short voice profile if voice matching matters
- the core angle
- platform-native drafts
- posting order only if it helps execution
- gaps that must be filled before publishing

## Quality Gate

Before delivering:
- every draft sounds like the intended author, not the platform stereotype
- every draft contains a real claim, proof point, or concrete observation
- no generic hype language remains
- no fake engagement bait remains
- no duplicated copy across platforms unless requested
- any CTA is earned and user-approved

## Related Skills

- `brand-voice` for source-derived voice profiles
- `crosspost` for platform-specific distribution
- `x-api` for sourcing recent posts and publishing approved X output
