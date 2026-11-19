---
id: everything-claude-code__rails-security
name: rails-security
version: 1.0.0
description: >-
  Ruby on Rails security practices for Rails 7.1+ and 8.x apps. Covers production configuration, authentication, authorization, strong parameters, SQL injection, XSS and output escaping, CSRF, file uploads, API security, credentials, untrusted boundaries, and dependency scanning. Use when reviewing or writing Rails authentication, authorization, input handling, uploads, or deployment configuration.
role: rails-security
category: security
triggers:
  - rails security
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/rails-security/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: rails-security
---

# rails-security

## Role

Portable distillation of upstream skill `rails-security` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Ruby on Rails security practices for Rails 7.1+ and 8.x apps. Covers production configuration, authentication, authorization, strong parameters, SQL injection, XSS and output escaping, CSRF, file uploads, API security, credentials, untrusted boundaries, and dependency scanning. Use when reviewing or writing Rails authentication, authorization, input handling, uploads, or deployment configuration.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
