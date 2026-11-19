---
id: everything-claude-code__kotlin-patterns
name: kotlin-patterns
version: 1.0.0
description: >-
  Idiomatic Kotlin patterns, best practices, and conventions for building robust, efficient, and maintainable Kotlin applications with coroutines, null safety, and DSL builders. Use when writing or reviewing Kotlin code and idiomatic structure or null safety is in question.
role: kotlin-patterns
category: design
triggers:
  - kotlin patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - test.run
sources:
  - research/everything-claude-code/skills/kotlin-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: kotlin-patterns
---

# kotlin-patterns

## Role

Portable distillation of upstream skill `kotlin-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Idiomatic Kotlin patterns, best practices, and conventions for building robust, efficient, and maintainable Kotlin applications with coroutines, null safety, and DSL builders. Use when writing or reviewing Kotlin code and idiomatic structure or null safety is in question.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
