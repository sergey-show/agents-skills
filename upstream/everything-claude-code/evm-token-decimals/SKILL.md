---
id: everything-claude-code__evm-token-decimals
name: evm-token-decimals
version: 1.0.0
description: >-
  Prevent silent decimal mismatch bugs across EVM chains. Covers runtime decimal lookup, chain-aware caching, bridged-token precision drift, and safe normalization for bots, dashboards, and DeFi tools. Use when handling token amounts across EVM chains, or when a balance, price, or transfer amount is off by orders of magnitude.
role: evm-token-decimals
category: ops
triggers:
  - evm token decimals
capabilities_required:
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/evm-token-decimals/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: evm-token-decimals
---

# evm-token-decimals

## Role

Portable distillation of upstream skill `evm-token-decimals` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Prevent silent decimal mismatch bugs across EVM chains. Covers runtime decimal lookup, chain-aware caching, bridged-token precision drift, and safe normalization for bots, dashboards, and DeFi tools. Use when handling token amounts across EVM chains, or when a balance, price, or transfer amount is off by orders of magnitude.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
