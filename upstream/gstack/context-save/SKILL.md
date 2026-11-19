---
id: gstack__context-save
name: context-save
version: 1.0.0
description: >-
  Save working context. Use for: save progress, save state, save my work, context save. (gstack)
role: context-save
category: meta
triggers:
  - context save
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
sources:
  - research/gstack/context-save/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: context-save
---

# context-save

## Role

Portable distillation of upstream skill `context-save` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Save working context. Use for: save progress, save state, save my work, context save. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
