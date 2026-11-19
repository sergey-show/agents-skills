---
id: everything-claude-code__ecc-conventions
name: ecc-conventions
version: 1.0.0
description: >-
  Development conventions and patterns for ECC. JavaScript project with conventional commits.
role: ecc-conventions
category: meta
triggers:
  - ecc conventions
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/ecc-conventions/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ecc-conventions
---

# ecc-conventions

## Role

Portable distillation of upstream skill `ecc-conventions` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Development conventions and patterns for ECC. JavaScript project with conventional commits.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
