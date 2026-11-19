---
id: everything-claude-code__defi-amm-security
name: defi-amm-security
version: 1.0.0
description: >-
  Security checklist for Solidity AMM contracts, liquidity pools, and swap flows. Covers reentrancy, CEI ordering, donation or inflation attacks, oracle manipulation, slippage, admin controls, and integer math. Use when auditing or writing Solidity AMM, liquidity pool, or swap code.
role: defi-amm-security
category: security
triggers:
  - defi amm security
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/defi-amm-security/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: defi-amm-security
---

# defi-amm-security

## Role

Portable distillation of upstream skill `defi-amm-security` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Security checklist for Solidity AMM contracts, liquidity pools, and swap flows. Covers reentrancy, CEI ordering, donation or inflation attacks, oracle manipulation, slippage, admin controls, and integer math. Use when auditing or writing Solidity AMM, liquidity pool, or swap code.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
