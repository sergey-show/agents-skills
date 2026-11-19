---
id: gstack__learn
name: learn
version: 1.0.0
description: >-
  Manage project learnings. Use for: show learnings, what have we learned.
role: learn
category: meta
triggers:
  - learn
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/learn/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: learn
---

# learn

## Role

Portable distillation of upstream skill `learn` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Manage project learnings. Use for: show learnings, what have we learned.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
