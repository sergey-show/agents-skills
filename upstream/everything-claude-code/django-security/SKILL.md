---
id: everything-claude-code__django-security
name: django-security
version: 1.0.0
description: >-
  Django security best practices, authentication, authorization, CSRF protection, SQL injection prevention, XSS prevention, and secure deployment configurations. Use when reviewing Django authentication, authorization, input handling, or deployment settings.
role: django-security
category: security
triggers:
  - django security
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/django-security/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: django-security
---

# django-security

## Role

Portable distillation of upstream skill `django-security` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Django security best practices, authentication, authorization, CSRF protection, SQL injection prevention, XSS prevention, and secure deployment configurations. Use when reviewing Django authentication, authorization, input handling, or deployment settings.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
