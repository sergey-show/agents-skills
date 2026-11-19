---
id: everything-claude-code__data-throughput-accelerator
name: data-throughput-accelerator
version: 1.0.0
description: >-
  Diagnose and accelerate large data movement — ingestion, backfill, export, ETL, warehouse loading, manifest catch-up, and table synchronization — by isolating the true bottleneck, benchmarking variants, and codifying the fastest path with a hard accounting block proving rows and timestamps cohere. Use when a pipeline or backfill is too slow and must get faster without losing data correctness.
role: data-throughput-accelerator
category: meta
triggers:
  - data throughput accelerator
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/data-throughput-accelerator/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: data-throughput-accelerator
---

# data-throughput-accelerator

## Role

Portable distillation of upstream skill `data-throughput-accelerator` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Diagnose and accelerate large data movement — ingestion, backfill, export, ETL, warehouse loading, manifest catch-up, and table synchronization — by isolating the true bottleneck, benchmarking variants, and codifying the fastest path with a hard accounting block proving rows and timestamps cohere. Use when a pipeline or backfill is too slow and must get faster without losing data correctness.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
