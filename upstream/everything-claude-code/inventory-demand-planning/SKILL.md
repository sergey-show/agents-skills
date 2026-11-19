---
id: everything-claude-code__inventory-demand-planning
name: inventory-demand-planning
version: 1.0.0
description: >-
  Codified demand planning expertise for multi-location retailers: demand forecasting method selection, ABC/XYZ segmentation, safety stock and reorder-point optimization, promotional lift and post-promo dip estimation, and seasonal transition and markdown timing. Use when forecasting demand, setting safety stock, planning replenishment, managing promotions, or optimizing inventory levels.
role: inventory-demand-planning
category: engineering
triggers:
  - inventory demand planning
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
sources:
  - research/everything-claude-code/skills/inventory-demand-planning/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: inventory-demand-planning
---

# inventory-demand-planning

## Role

Portable distillation of upstream skill `inventory-demand-planning` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Codified demand planning expertise for multi-location retailers: demand forecasting method selection, ABC/XYZ segmentation, safety stock and reorder-point optimization, promotional lift and post-promo dip estimation, and seasonal transition and markdown timing. Use when forecasting demand, setting safety stock, planning replenishment, managing promotions, or optimizing inventory levels.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
