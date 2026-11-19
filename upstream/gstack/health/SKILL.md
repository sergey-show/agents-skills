---
id: gstack__health
name: health
version: 1.0.0
description: >-
  Code quality dashboard. Use for: code health check, quality dashboard. (gstack)
role: health
category: meta
triggers:
  - health
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
  - research/gstack/health/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: health
---

# health

## Role

Portable distillation of upstream skill `health` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Code quality dashboard. Use for: code health check, quality dashboard. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
