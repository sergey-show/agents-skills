---
id: everything-claude-code__django-celery
name: django-celery
version: 1.0.0
description: >-
  Django + Celery async task patterns — configuration, task design, beat scheduling, retries, canvas workflows, monitoring, and testing. Use when adding background jobs, scheduled tasks, or async processing to a Django app.
role: django-celery
category: engineering
triggers:
  - django celery
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/django-celery/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: django-celery
---

# django-celery

## Role

Portable distillation of upstream skill `django-celery` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Django + Celery async task patterns — configuration, task design, beat scheduling, retries, canvas workflows, monitoring, and testing. Use when adding background jobs, scheduled tasks, or async processing to a Django app.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
