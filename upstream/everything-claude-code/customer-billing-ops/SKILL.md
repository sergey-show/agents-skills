---
id: everything-claude-code__customer-billing-ops
name: customer-billing-ops
version: 1.0.0
description: >-
  Operate customer billing workflows such as subscriptions, refunds, churn triage, billing-portal recovery, and plan analysis using connected billing tools like Stripe. Use when the user needs to help a customer, inspect subscription state, or manage revenue-impacting billing operations.
role: customer-billing-ops
category: design
triggers:
  - customer billing ops
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
sources:
  - research/everything-claude-code/skills/customer-billing-ops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: customer-billing-ops
---

# customer-billing-ops

## Role

Portable distillation of upstream skill `customer-billing-ops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Operate customer billing workflows such as subscriptions, refunds, churn triage, billing-portal recovery, and plan analysis using connected billing tools like Stripe. Use when the user needs to help a customer, inspect subscription state, or manage revenue-impacting billing operations.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
