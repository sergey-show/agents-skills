---
id: everything-claude-code__agent-payment-x402
name: agent-payment-x402
version: 1.0.0
description: >-
  Add x402 payment execution to AI agents with per-task budgets, spending controls, and non-custodial wallets. Supports Base through agentwallet-sdk, X Layer through OKX Payments / OKX Agent Payments Protocol, and Solana plus multi-network EVM through the upstream x402 packages with facilitator-based settlement. Use when an agent must pay for something itself and needs per-task budgets, spending controls, and a non-custodial wallet.
role: agent-payment-x402
category: security
triggers:
  - agent payment x402
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/agent-payment-x402/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agent-payment-x402
---

# agent-payment-x402

## Role

Portable distillation of upstream skill `agent-payment-x402` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Add x402 payment execution to AI agents with per-task budgets, spending controls, and non-custodial wallets. Supports Base through agentwallet-sdk, X Layer through OKX Payments / OKX Agent Payments Protocol, and Solana plus multi-network EVM through the upstream x402 packages with facilitator-based settlement. Use when an agent must pay for something itself and needs per-task budgets, spending controls, and a non-custodial wallet.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
