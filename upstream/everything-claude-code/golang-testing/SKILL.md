---
id: everything-claude-code__golang-testing
name: golang-testing
version: 1.0.0
description: >-
  Go testing patterns including table-driven tests, subtests, benchmarks, fuzzing, and test coverage. Follows TDD methodology with idiomatic Go practices. Use when writing Go tests — table-driven cases, subtests, benchmarks, fuzzing, or coverage.
role: golang-testing
category: engineering
triggers:
  - golang testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/golang-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: golang-testing
---

# golang-testing

## Role

Portable distillation of upstream skill `golang-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Go testing patterns including table-driven tests, subtests, benchmarks, fuzzing, and test coverage. Follows TDD methodology with idiomatic Go practices. Use when writing Go tests — table-driven cases, subtests, benchmarks, fuzzing, or coverage.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
