---
id: everything-claude-code__dashboard-builder
name: dashboard-builder
version: 1.0.0
description: >-
  Build monitoring dashboards that answer real operator questions for Grafana, SigNoz, and similar platforms. Use when turning metrics into a working dashboard instead of a vanity board.
role: dashboard-builder
category: engineering
triggers:
  - dashboard builder
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/dashboard-builder/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: dashboard-builder
---

# dashboard-builder

## Role

Portable distillation of upstream skill `dashboard-builder` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build monitoring dashboards that answer real operator questions for Grafana, SigNoz, and similar platforms. Use when turning metrics into a working dashboard instead of a vanity board.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
