---
id: everything-claude-code__growth-log
name: growth-log
version: 1.0.0
description: >-
  Write growth log entries that extract reusable patterns from completed work — root cause, transferable rule, and a recognizable signal — instead of diary-style event narration, with a 4-8 sentence template and merge-duplicates discipline. Use when capturing what was learned after a complex task, debugging session, failure, or rollback, when reviewing progress over a period, or when a delivery gate asks what was learned.
role: growth-log
category: meta
triggers:
  - growth log
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
sources:
  - research/everything-claude-code/skills/growth-log/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: growth-log
---

# growth-log

## Role

Portable distillation of upstream skill `growth-log` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Write growth log entries that extract reusable patterns from completed work — root cause, transferable rule, and a recognizable signal — instead of diary-style event narration, with a 4-8 sentence template and merge-duplicates discipline. Use when capturing what was learned after a complex task, debugging session, failure, or rollback, when reviewing progress over a period, or when a delivery gate asks what was learned.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
