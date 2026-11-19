---
id: everything-claude-code__production-scheduling
name: production-scheduling
version: 1.0.0
description: >-
  Codified expertise for production scheduling, job sequencing, line balancing, changeover optimization, and bottleneck resolution in discrete and batch manufacturing. Informed by production schedulers with 15+ years experience. Includes TOC/drum-buffer-rope, SMED, OEE analysis, disruption response frameworks, and ERP/MES interaction patterns. Use when scheduling production, resolving bottlenecks, optimizing changeovers, responding to disruptions, or balancing manufacturing lines.
role: production-scheduling
category: engineering
triggers:
  - production scheduling
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/production-scheduling/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: production-scheduling
---

# production-scheduling

## Role

Portable distillation of upstream skill `production-scheduling` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Codified expertise for production scheduling, job sequencing, line balancing, changeover optimization, and bottleneck resolution in discrete and batch manufacturing. Informed by production schedulers with 15+ years experience. Includes TOC/drum-buffer-rope, SMED, OEE analysis, disruption response frameworks, and ERP/MES interaction patterns. Use when scheduling production, resolving bottlenecks, optimizing changeovers, responding to disruptions, or balancing manufacturing lines.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
