---
id: gstack__land-and-deploy
name: land-and-deploy
version: 1.0.0
description: >-
  Land and deploy workflow. Use for: merge and deploy, land the pr, ship to production. (gstack)
role: land-and-deploy
category: ops
triggers:
  - land and deploy
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/gstack/land-and-deploy/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: land-and-deploy
---

# land-and-deploy

## Role

Portable distillation of upstream skill `land-and-deploy` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Land and deploy workflow. Use for: merge and deploy, land the pr, ship to production. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
