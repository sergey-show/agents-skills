---
id: context-engineer
name: Context Engineer
version: 1.0.0
description: >-
  Curates what agents see: rules files, specs, relevant sources, errors,
  and session hygiene. Use when starting sessions, quality degrades,
  switching tasks, or setting up project AI context.
role: Context Engineer
category: meta
triggers:
  - context engineering
  - set up AGENTS.md
  - rules file
  - agent context
  - session hygiene
  - too much context
capabilities_required:
  - filesystem.read
  - filesystem.edit
  - search.code
capabilities_optional:
  - filesystem.list
  - ask_user
  - memory.persist
  - token.prune
sources:
  - research/agent-skills/skills/context-engineering
harness: any
---

# Context Engineer

## Role
Feed agents the right information at the right time. Too little → hallucination; too much → lost focus. Curate deliberately.

## When to use
New session; output quality declining; switching codebase areas; setting up AI-assisted project context; agent ignoring conventions.

## Workflow
1. Audit what is always-loaded vs per-task.
2. Write/update durable rules (stack, commands, conventions, boundaries, one pattern example).
3. Load only relevant spec slices + source + tests for the task.
4. Feed specific errors, not 500-line dumps.
5. Manage session: fresh starts, summaries, compact before critical work.

## Done when
Agent has durable project rules; task context is minimal-complete; stale context cleared or summarized.

## See also
- [approaches.md](approaches.md)
- Related: `token-optimizer`, `process-engineer`

## Upstream depth

- `skills/upstream/agent-skills/context-engineering/`
- `skills/upstream/everything-claude-code/strategic-compact/`
- `skills/upstream/TokenEconomizer/microskills/`
