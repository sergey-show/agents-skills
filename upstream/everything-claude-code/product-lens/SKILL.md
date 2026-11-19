---
id: everything-claude-code__product-lens
name: product-lens
version: 1.0.0
description: >-
  Validate the why before building through four product diagnostics — a YC-style product diagnostic that produces PRODUCT-BRIEF.md with a go/no-go recommendation, a founder review scoring product-market-fit signals, a user journey audit measuring time-to-value, and ICE feature prioritization. Use when pressure-testing product direction, choosing between features, sanity-checking a launch, or converting a vague idea into a product brief.
role: product-lens
category: engineering
triggers:
  - product lens
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
sources:
  - research/everything-claude-code/skills/product-lens/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: product-lens
---

# product-lens

## Role

Portable distillation of upstream skill `product-lens` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Validate the why before building through four product diagnostics — a YC-style product diagnostic that produces PRODUCT-BRIEF.md with a go/no-go recommendation, a founder review scoring product-market-fit signals, a user journey audit measuring time-to-value, and ICE feature prioritization. Use when pressure-testing product direction, choosing between features, sanity-checking a launch, or converting a vague idea into a product brief.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
