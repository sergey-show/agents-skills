---
id: everything-claude-code__prediction-market-oracle-research
name: prediction-market-oracle-research
version: 1.0.0
description: >-
  Research prediction markets as data sources or oracle signals for products, agents, dashboards, and corporate decision intelligence. Use for source-grounded analysis of market-implied probabilities, caveats, and integration patterns without investment advice. Use when evaluating prediction markets as a data source or oracle signal for a product, agent, or dashboard.
role: prediction-market-oracle-research
category: research
triggers:
  - prediction market oracle research
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/prediction-market-oracle-research/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: prediction-market-oracle-research
---

# prediction-market-oracle-research

## Role

Portable distillation of upstream skill `prediction-market-oracle-research` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Research prediction markets as data sources or oracle signals for products, agents, dashboards, and corporate decision intelligence. Use for source-grounded analysis of market-implied probabilities, caveats, and integration patterns without investment advice. Use when evaluating prediction markets as a data source or oracle signal for a product, agent, or dashboard.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
