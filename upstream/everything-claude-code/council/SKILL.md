---
id: everything-claude-code__council
name: council
version: 1.0.0
description: >-
  Convene a four-voice council for ambiguous decisions, tradeoffs, and go/no-go calls. Use when multiple valid paths exist and you need structured disagreement before choosing.
role: council
category: design
triggers:
  - council
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/council/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: council
---

# council

## Role

Portable distillation of upstream skill `council` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Convene a four-voice council for ambiguous decisions, tradeoffs, and go/no-go calls. Use when multiple valid paths exist and you need structured disagreement before choosing.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
