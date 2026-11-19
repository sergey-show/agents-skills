---
id: gstack__canary
name: canary
version: 1.0.0
description: >-
  Post-deploy canary monitoring. Use for: monitor after deploy, canary check. (gstack)
role: canary
category: ops
triggers:
  - canary
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
  - research/gstack/canary/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: canary
---

# canary

## Role

Portable distillation of upstream skill `canary` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Post-deploy canary monitoring. Use for: monitor after deploy, canary check. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
