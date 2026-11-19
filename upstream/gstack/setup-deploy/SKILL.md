---
id: gstack__setup-deploy
name: setup-deploy
version: 1.0.0
description: >-
  Configure deployment settings for /land-and-deploy. Use for: configure deploy, setup deployment.
role: setup-deploy
category: ops
triggers:
  - setup deploy
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
sources:
  - research/gstack/setup-deploy/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: setup-deploy
---

# setup-deploy

## Role

Portable distillation of upstream skill `setup-deploy` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Configure deployment settings for /land-and-deploy. Use for: configure deploy, setup deployment.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
