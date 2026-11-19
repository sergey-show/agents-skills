---
id: everything-claude-code__prisma-patterns
name: prisma-patterns
version: 1.0.0
description: >-
  Prisma ORM patterns for TypeScript backends — schema design, query optimization, transactions, pagination, and critical traps like updateMany returning count not records, $transaction timeouts, migrate dev resetting the DB, @updatedAt skipped on bulk writes, and serverless connection exhaustion. Use when writing a Prisma schema or query, or debugging transactions, migrations, or serverless connection limits.
role: prisma-patterns
category: ops
triggers:
  - prisma patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/prisma-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: prisma-patterns
---

# prisma-patterns

## Role

Portable distillation of upstream skill `prisma-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Prisma ORM patterns for TypeScript backends — schema design, query optimization, transactions, pagination, and critical traps like updateMany returning count not records, $transaction timeouts, migrate dev resetting the DB, @updatedAt skipped on bulk writes, and serverless connection exhaustion. Use when writing a Prisma schema or query, or debugging transactions, migrations, or serverless connection limits.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
