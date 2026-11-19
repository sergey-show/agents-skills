---
id: everything-claude-code__finance-billing-ops
name: finance-billing-ops
version: 1.0.0
description: >-
  Evidence-first revenue, pricing, refunds, team-billing, and billing-model truth workflow for ECC. Use when the user wants a sales snapshot, pricing comparison, duplicate-charge diagnosis, or code-backed billing reality instead of generic payments advice.
role: finance-billing-ops
category: meta
triggers:
  - finance billing ops
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/finance-billing-ops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: finance-billing-ops
---

# finance-billing-ops

## Role

Portable distillation of upstream skill `finance-billing-ops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Evidence-first revenue, pricing, refunds, team-billing, and billing-model truth workflow for ECC. Use when the user wants a sales snapshot, pricing comparison, duplicate-charge diagnosis, or code-backed billing reality instead of generic payments advice.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
