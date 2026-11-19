---
id: gstack__careful
name: careful
version: 1.0.0
description: >-
  Safety guardrails for destructive commands. Use for: be careful, warn before destructive, safety mode. (gstack)
role: careful
category: meta
triggers:
  - careful
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
sources:
  - research/gstack/careful/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: careful
---

# careful

## Role

Portable distillation of upstream skill `careful` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Safety guardrails for destructive commands. Use for: be careful, warn before destructive, safety mode. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
