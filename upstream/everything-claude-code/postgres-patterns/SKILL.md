---
id: everything-claude-code__postgres-patterns
name: postgres-patterns
version: 1.0.0
description: >-
  PostgreSQL database patterns for query optimization, schema design, indexing, and security. Based on Supabase best practices. Use when designing PostgreSQL schemas, indexes, or RLS policies, or when a query is too slow.
role: postgres-patterns
category: design
triggers:
  - postgres patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/postgres-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: postgres-patterns
---

# postgres-patterns

## Role

Portable distillation of upstream skill `postgres-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

PostgreSQL database patterns for query optimization, schema design, indexing, and security. Based on Supabase best practices. Use when designing PostgreSQL schemas, indexes, or RLS policies, or when a query is too slow.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
