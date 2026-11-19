---
id: everything-claude-code__ito-baskets
name: ito-baskets
version: 1.0.0
description: >-
  Read-only Itô basket and prediction-market data skill. Index the live basket catalog, compare a basket against user-supplied research or a watchlist, build a source-grounded market brief, or draft a non-executable planning worksheet. Use when a user asks to browse or index Itô baskets, compare a basket against notes or a thesis, research prediction-market events/venues/liquidity, or plan a basket or market idea without trading. Never advises, orders, trades, reserves, or executes.
role: ito-baskets
category: research
triggers:
  - ito baskets
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/ito-baskets/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ito-baskets
---

# ito-baskets

## Role

Portable distillation of upstream skill `ito-baskets` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Read-only Itô basket and prediction-market data skill. Index the live basket catalog, compare a basket against user-supplied research or a watchlist, build a source-grounded market brief, or draft a non-executable planning worksheet. Use when a user asks to browse or index Itô baskets, compare a basket against notes or a thesis, research prediction-market events/venues/liquidity, or plan a basket or market idea without trading. Never advises, orders, trades, reserves, or executes.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
