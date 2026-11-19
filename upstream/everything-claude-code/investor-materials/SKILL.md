---
id: everything-claude-code__investor-materials
name: investor-materials
version: 1.0.0
description: >-
  Create and update pitch decks, one-pagers, investor memos, accelerator applications, financial models, and fundraising materials. Use when the user needs investor-facing documents, projections, use-of-funds tables, milestone plans, or materials that must stay internally consistent across multiple fundraising assets.
role: investor-materials
category: engineering
triggers:
  - investor materials
capabilities_required:
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/.agents/skills/investor-materials/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: investor-materials
---

# investor-materials

## Role

Portable distillation of upstream skill `investor-materials` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Create and update pitch decks, one-pagers, investor memos, accelerator applications, financial models, and fundraising materials. Use when the user needs investor-facing documents, projections, use-of-funds tables, milestone plans, or materials that must stay internally consistent across multiple fundraising assets.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
