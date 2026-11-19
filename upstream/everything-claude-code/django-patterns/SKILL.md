---
id: everything-claude-code__django-patterns
name: django-patterns
version: 1.0.0
description: >-
  Django architecture patterns, REST API design with DRF, ORM best practices, caching, signals, middleware, and production-grade Django apps. Use when building or reviewing Django apps, DRF APIs, ORM queries, or caching.
role: django-patterns
category: design
triggers:
  - django patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/django-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: django-patterns
---

# django-patterns

## Role

Portable distillation of upstream skill `django-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Django architecture patterns, REST API design with DRF, ORM best practices, caching, signals, middleware, and production-grade Django apps. Use when building or reviewing Django apps, DRF APIs, ORM queries, or caching.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
