---
id: superpowers__using-superpowers
name: using-superpowers
version: 1.0.0
description: >-
  Use when starting any conversation - establishes how to find and use skills, requiring skill invocation before ANY response including clarifying questions
role: using-superpowers
category: meta
triggers:
  - using superpowers
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - subagent.spawn
sources:
  - research/superpowers/skills/using-superpowers/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: using-superpowers
---

# using-superpowers

## Role

Portable distillation of upstream skill `using-superpowers` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when starting any conversation - establishes how to find and use skills, requiring skill invocation before ANY response including clarifying questions

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
