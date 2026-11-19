---
id: everything-claude-code__energy-procurement
name: energy-procurement
version: 1.0.0
description: >-
  Procure electricity and natural gas for commercial and industrial facilities: tariff and rate-schedule optimization, demand-charge mitigation, supplier RFPs, fixed/index/block-and-index hedging, renewable PPA and REC evaluation, and sustainability reporting. Use when procuring energy, optimizing utility tariffs, managing demand charges, evaluating PPAs, or building energy budgets and hedge strategies.
role: energy-procurement
category: research
triggers:
  - energy procurement
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/energy-procurement/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: energy-procurement
---

# energy-procurement

## Role

Portable distillation of upstream skill `energy-procurement` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Procure electricity and natural gas for commercial and industrial facilities: tariff and rate-schedule optimization, demand-charge mitigation, supplier RFPs, fixed/index/block-and-index hedging, renewable PPA and REC evaluation, and sustainability reporting. Use when procuring energy, optimizing utility tariffs, managing demand charges, evaluating PPAs, or building energy budgets and hedge strategies.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
