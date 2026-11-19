---
id: gstack__context-restore
name: context-restore
version: 1.0.0
description: >-
  Restore working context saved earlier by /context-save. Use for: resume where i left off, restore context, where was i. (gstack)
role: context-restore
category: meta
triggers:
  - context restore
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
  - research/gstack/context-restore/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: context-restore
---

# context-restore

## Role

Portable distillation of upstream skill `context-restore` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Restore working context saved earlier by /context-save. Use for: resume where i left off, restore context, where was i. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
