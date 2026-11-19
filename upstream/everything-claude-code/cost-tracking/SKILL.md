---
id: everything-claude-code__cost-tracking
name: cost-tracking
version: 1.0.0
description: >-
  Track and report the coding agent token usage, spending, and budgets from the local ECC cost-tracker metrics log. Use when the user asks about costs, spending, usage, tokens, budgets, or cost breakdowns by model, session, or date.
role: cost-tracking
category: meta
triggers:
  - cost tracking
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/cost-tracking/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: cost-tracking
---

# cost-tracking

## Role

Portable distillation of upstream skill `cost-tracking` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Track and report the coding agent token usage, spending, and budgets from the local ECC cost-tracker metrics log. Use when the user asks about costs, spending, usage, tokens, budgets, or cost breakdowns by model, session, or date.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
