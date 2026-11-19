---
id: everything-claude-code__agentic-engineering
name: agentic-engineering
version: 1.0.0
description: >-
  Operate as an agentic engineer using eval-first execution, decomposition, and cost-aware model routing. Use when planning or executing engineering work that agents will carry out end to end.
role: agentic-engineering
category: meta
triggers:
  - agentic engineering
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/agentic-engineering/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agentic-engineering
---

# agentic-engineering

## Role

Portable distillation of upstream skill `agentic-engineering` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Operate as an agentic engineer using eval-first execution, decomposition, and cost-aware model routing. Use when planning or executing engineering work that agents will carry out end to end.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
