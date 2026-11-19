---
id: everything-claude-code__recursive-decision-ledger
name: recursive-decision-ledger
version: 1.0.0
description: >-
  Run repeated rollouts ("Prime Gauss" style recursive prompting) while keeping an append-only decision ledger of trials, marks, coherence checks, and promotion gates, so recursive confidence never auto-approves live trading, deploy, or destructive actions. Use when the user asks for repeated rollouts, marked decision processes, high-dimensional search, stochastic optimization, local-optima exploration, ensemble comparison, or recursive reasoning with a visible evidence trail.
role: recursive-decision-ledger
category: meta
triggers:
  - recursive decision ledger
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - test.run
sources:
  - research/everything-claude-code/skills/recursive-decision-ledger/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: recursive-decision-ledger
---

# recursive-decision-ledger

## Role

Portable distillation of upstream skill `recursive-decision-ledger` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Run repeated rollouts ("Prime Gauss" style recursive prompting) while keeping an append-only decision ledger of trials, marks, coherence checks, and promotion gates, so recursive confidence never auto-approves live trading, deploy, or destructive actions. Use when the user asks for repeated rollouts, marked decision processes, high-dimensional search, stochastic optimization, local-optima exploration, ensemble comparison, or recursive reasoning with a visible evidence trail.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
