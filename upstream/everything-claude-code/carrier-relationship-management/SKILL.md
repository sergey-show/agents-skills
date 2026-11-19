---
id: everything-claude-code__carrier-relationship-management
name: carrier-relationship-management
version: 1.0.0
description: >-
  Manage truckload, LTL, and intermodal carrier portfolios: sourcing and FMCSA vetting, freight rate and fuel-surcharge negotiation, RFPs and routing guides, carrier scorecards, allocation, and renewals. Use when onboarding carriers, running freight RFPs, negotiating rates, evaluating carrier performance, reallocating freight, or building freight strategy.
role: carrier-relationship-management
category: ops
triggers:
  - carrier relationship management
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/carrier-relationship-management/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: carrier-relationship-management
---

# carrier-relationship-management

## Role

Portable distillation of upstream skill `carrier-relationship-management` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Manage truckload, LTL, and intermodal carrier portfolios: sourcing and FMCSA vetting, freight rate and fuel-surcharge negotiation, RFPs and routing guides, carrier scorecards, allocation, and renewals. Use when onboarding carriers, running freight RFPs, negotiating rates, evaluating carrier performance, reallocating freight, or building freight strategy.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
