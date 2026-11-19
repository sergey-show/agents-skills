---
id: everything-claude-code__kotlin-testing
name: kotlin-testing
version: 1.0.0
description: >-
  Kotlin testing patterns with Kotest, MockK, coroutine testing, property-based testing, and Kover coverage. Follows TDD methodology with idiomatic Kotlin practices. Use when writing Kotlin tests with Kotest or MockK, or testing coroutines and checking coverage.
role: kotlin-testing
category: engineering
triggers:
  - kotlin testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/kotlin-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: kotlin-testing
---

# kotlin-testing

## Role

Portable distillation of upstream skill `kotlin-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Kotlin testing patterns with Kotest, MockK, coroutine testing, property-based testing, and Kover coverage. Follows TDD methodology with idiomatic Kotlin practices. Use when writing Kotlin tests with Kotest or MockK, or testing coroutines and checking coverage.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
