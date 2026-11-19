---
id: everything-claude-code__laravel-verification
name: laravel-verification
version: 1.0.0
description: >-
  Verification loop for Laravel projects: env checks, linting, static analysis, tests with coverage, security scans, and deployment readiness. Use when verifying a Laravel project before merge or deploy — lint, static analysis, tests, coverage, security.
role: laravel-verification
category: security
triggers:
  - laravel verification
capabilities_required:
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/laravel-verification/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: laravel-verification
---

# laravel-verification

## Role

Portable distillation of upstream skill `laravel-verification` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Verification loop for Laravel projects: env checks, linting, static analysis, tests with coverage, security scans, and deployment readiness. Use when verifying a Laravel project before merge or deploy — lint, static analysis, tests, coverage, security.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
