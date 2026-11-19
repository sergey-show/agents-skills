---
id: everything-claude-code__config-health
name: config-health
version: 1.0.0
description: >-
  Runtime configuration integrity monitoring for the coding agent. Detects config drift, rule staleness, and hook wiring gaps at startup, with an optional per-tool mode. Complements delivery-gate with startup soft monitoring.
role: config-health
category: engineering
triggers:
  - config health
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/config-health/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: config-health
---

# config-health

## Role

Portable distillation of upstream skill `config-health` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Runtime configuration integrity monitoring for the coding agent. Detects config drift, rule staleness, and hook wiring gaps at startup, with an optional per-tool mode. Complements delivery-gate with startup soft monitoring.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
