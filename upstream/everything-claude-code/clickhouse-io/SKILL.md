---
id: everything-claude-code__clickhouse-io
name: clickhouse-io
version: 1.0.0
description: >-
  ClickHouse database patterns, query optimization, analytics, and data engineering best practices for high-performance analytical workloads. Use when writing ClickHouse schemas or queries, or when an analytical query is too slow.
role: clickhouse-io
category: design
triggers:
  - clickhouse io
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/clickhouse-io/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: clickhouse-io
---

# clickhouse-io

## Role

Portable distillation of upstream skill `clickhouse-io` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

ClickHouse database patterns, query optimization, analytics, and data engineering best practices for high-performance analytical workloads. Use when writing ClickHouse schemas or queries, or when an analytical query is too slow.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
