---
id: gstack__gstack-upgrade
name: gstack-upgrade
version: 1.0.0
description: >-
  Upgrade gstack to the latest version. Use for: upgrade gstack, update gstack version.
role: gstack-upgrade
category: meta
triggers:
  - gstack upgrade
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/gstack/gstack-upgrade/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: gstack-upgrade
---

# gstack-upgrade

## Role

Portable distillation of upstream skill `gstack-upgrade` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Upgrade gstack to the latest version. Use for: upgrade gstack, update gstack version.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
