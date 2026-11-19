---
id: everything-claude-code__mysql-patterns
name: mysql-patterns
version: 1.0.0
description: >-
  MySQL and MariaDB schema, query, indexing, transaction, replication, and connection-pool patterns for production backends. Use when designing MySQL or MariaDB schemas and indexes, or when a query, transaction, or replica lags.
role: mysql-patterns
category: design
triggers:
  - mysql patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/mysql-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: mysql-patterns
---

# mysql-patterns

## Role

Portable distillation of upstream skill `mysql-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

MySQL and MariaDB schema, query, indexing, transaction, replication, and connection-pool patterns for production backends. Use when designing MySQL or MariaDB schemas and indexes, or when a query, transaction, or replica lags.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
