---
id: gstack__retro
name: retro
version: 1.0.0
description: >-
  Weekly engineering retrospective. Use for: weekly retro, what did we ship. (gstack)
role: retro
category: meta
triggers:
  - retro
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
  - research/gstack/retro/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: retro
---

# retro

## Role

Portable distillation of upstream skill `retro` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Weekly engineering retrospective. Use for: weekly retro, what did we ship. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
