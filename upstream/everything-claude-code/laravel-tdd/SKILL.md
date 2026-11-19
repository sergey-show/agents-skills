---
id: everything-claude-code__laravel-tdd
name: laravel-tdd
version: 1.0.0
description: >-
  Laravel testing strategies with PHPUnit, Pest, model factories, HTTP tests, Sanctum authentication testing, mocking, and coverage. Use when writing Laravel tests with PHPUnit or Pest, or driving a Laravel feature test-first.
role: laravel-tdd
category: ops
triggers:
  - laravel tdd
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/laravel-tdd/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: laravel-tdd
---

# laravel-tdd

## Role

Portable distillation of upstream skill `laravel-tdd` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Laravel testing strategies with PHPUnit, Pest, model factories, HTTP tests, Sanctum authentication testing, mocking, and coverage. Use when writing Laravel tests with PHPUnit or Pest, or driving a Laravel feature test-first.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
