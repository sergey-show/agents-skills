---
id: everything-claude-code__laravel-security
name: laravel-security
version: 1.0.0
description: >-
  Laravel security best practices — authentication, authorization, Eloquent safety, CSRF, XSS prevention, API security, and secure deployment configurations. Use when reviewing Laravel auth, Eloquent safety, CSRF, XSS, API security, or deployment configuration.
role: laravel-security
category: security
triggers:
  - laravel security
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/laravel-security/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: laravel-security
---

# laravel-security

## Role

Portable distillation of upstream skill `laravel-security` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Laravel security best practices — authentication, authorization, Eloquent safety, CSRF, XSS prevention, API security, and secure deployment configurations. Use when reviewing Laravel auth, Eloquent safety, CSRF, XSS, API security, or deployment configuration.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
