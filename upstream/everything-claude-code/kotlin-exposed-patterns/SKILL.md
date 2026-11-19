---
id: everything-claude-code__kotlin-exposed-patterns
name: kotlin-exposed-patterns
version: 1.0.0
description: >-
  JetBrains Exposed ORM patterns including DSL queries, DAO pattern, transactions, HikariCP connection pooling, Flyway migrations, and repository pattern. Use when working with the Exposed ORM — DSL or DAO queries, transactions, pooling, or migrations.
role: kotlin-exposed-patterns
category: engineering
triggers:
  - kotlin exposed patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/kotlin-exposed-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: kotlin-exposed-patterns
---

# kotlin-exposed-patterns

## Role

Portable distillation of upstream skill `kotlin-exposed-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

JetBrains Exposed ORM patterns including DSL queries, DAO pattern, transactions, HikariCP connection pooling, Flyway migrations, and repository pattern. Use when working with the Exposed ORM — DSL or DAO queries, transactions, pooling, or migrations.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
