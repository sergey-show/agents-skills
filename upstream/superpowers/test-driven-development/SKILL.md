---
id: superpowers__test-driven-development
name: test-driven-development
version: 1.0.0
description: >-
  Use when implementing any feature or bugfix, before writing implementation code
role: test-driven-development
category: engineering
triggers:
  - test driven development
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/superpowers/skills/test-driven-development/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: test-driven-development
---

# test-driven-development

## Role

Portable distillation of upstream skill `test-driven-development` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when implementing any feature or bugfix, before writing implementation code

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
