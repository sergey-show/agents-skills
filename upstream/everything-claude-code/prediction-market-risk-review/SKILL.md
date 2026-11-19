---
id: everything-claude-code__prediction-market-risk-review
name: prediction-market-risk-review
version: 1.0.0
description: >-
  Review prediction-market, basket, oracle, and trading-agent workflows for compliance, safety, data-quality, privacy, and execution risk. Use before any workflow handles venue auth, user portfolio data, API keys, or trade planning.
role: prediction-market-risk-review
category: research
triggers:
  - prediction market risk review
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
sources:
  - research/everything-claude-code/skills/prediction-market-risk-review/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: prediction-market-risk-review
---

# prediction-market-risk-review

## Role

Portable distillation of upstream skill `prediction-market-risk-review` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Review prediction-market, basket, oracle, and trading-agent workflows for compliance, safety, data-quality, privacy, and execution risk. Use before any workflow handles venue auth, user portfolio data, API keys, or trade planning.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
