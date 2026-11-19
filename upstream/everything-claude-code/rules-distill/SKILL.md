---
id: everything-claude-code__rules-distill
name: rules-distill
version: 1.0.0
description: >-
  Scan skills to extract cross-cutting principles and distill them into rules — append, revise, or create new rule files. Use when the same principle keeps recurring across skills and belongs in a rule file instead.
role: rules-distill
category: meta
triggers:
  - rules distill
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/rules-distill/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: rules-distill
---

# rules-distill

## Role

Portable distillation of upstream skill `rules-distill` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Scan skills to extract cross-cutting principles and distill them into rules — append, revise, or create new rule files. Use when the same principle keeps recurring across skills and belongs in a rule file instead.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
