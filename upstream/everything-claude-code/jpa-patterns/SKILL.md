---
id: everything-claude-code__jpa-patterns
name: jpa-patterns
version: 1.0.0
description: >-
  JPA/Hibernate patterns for entity design, relationships, query optimization, transactions, auditing, indexing, pagination, and pooling in Spring Boot. Use when designing JPA entities or relationships, or when a Hibernate query, transaction, or N+1 problem needs fixing.
role: jpa-patterns
category: design
triggers:
  - jpa patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/jpa-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: jpa-patterns
---

# jpa-patterns

## Role

Portable distillation of upstream skill `jpa-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

JPA/Hibernate patterns for entity design, relationships, query optimization, transactions, auditing, indexing, pagination, and pooling in Spring Boot. Use when designing JPA entities or relationships, or when a Hibernate query, transaction, or N+1 problem needs fixing.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
