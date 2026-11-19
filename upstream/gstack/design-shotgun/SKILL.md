---
id: gstack__design-shotgun
name: design-shotgun
version: 1.0.0
description: >-
  Design shotgun: generate multiple AI design variants, open a comparison board, collect structured feedback, and iterate. Use for: explore design variants, show me design options. (gstack)
role: design-shotgun
category: design
triggers:
  - design shotgun
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/design-shotgun/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: design-shotgun
---

# design-shotgun

## Role

Portable distillation of upstream skill `design-shotgun` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design shotgun: generate multiple AI design variants, open a comparison board, collect structured feedback, and iterate. Use for: explore design variants, show me design options. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
