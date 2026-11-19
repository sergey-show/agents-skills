---
id: gstack__guard
name: guard
version: 1.0.0
description: >-
  Full safety mode: destructive command warnings + directory-scoped edits. Use for: full safety mode, guard against mistakes. (gstack)
role: guard
category: meta
triggers:
  - guard
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
sources:
  - research/gstack/guard/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: guard
---

# guard

## Role

Portable distillation of upstream skill `guard` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Full safety mode: destructive command warnings + directory-scoped edits. Use for: full safety mode, guard against mistakes. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
