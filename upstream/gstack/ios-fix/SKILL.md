---
id: gstack__ios-fix
name: ios-fix
version: 1.0.0
description: >-
  Autonomous iOS bug fixer. Use for: fix this ios bug, patch the iphone app. (gstack)
role: ios-fix
category: meta
triggers:
  - ios fix
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/ios-fix/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: ios-fix
---

# ios-fix

## Role

Portable distillation of upstream skill `ios-fix` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Autonomous iOS bug fixer. Use for: fix this ios bug, patch the iphone app. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
