---
id: superpowers__requesting-code-review
name: requesting-code-review
version: 1.0.0
description: >-
  Use when completing tasks, implementing major features, or before merging to verify work meets requirements
role: requesting-code-review
category: meta
triggers:
  - requesting code review
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/superpowers/skills/requesting-code-review/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: requesting-code-review
---

# requesting-code-review

## Role

Portable distillation of upstream skill `requesting-code-review` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when completing tasks, implementing major features, or before merging to verify work meets requirements

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
