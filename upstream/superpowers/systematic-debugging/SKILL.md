---
id: superpowers__systematic-debugging
name: systematic-debugging
version: 1.0.0
description: >-
  Use when encountering any bug, test failure, or unexpected behavior, before proposing fixes
role: systematic-debugging
category: engineering
triggers:
  - systematic debugging
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
  - research/superpowers/skills/systematic-debugging/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: systematic-debugging
---

# systematic-debugging

## Role

Portable distillation of upstream skill `systematic-debugging` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when encountering any bug, test failure, or unexpected behavior, before proposing fixes

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
