---
id: everything-claude-code__product-capability
name: product-capability
version: 1.0.0
description: >-
  Translate PRD intent, roadmap asks, or product discussions into an implementation-ready capability plan that exposes constraints, invariants, interfaces, and unresolved decisions before multi-service work starts. Use when the user needs an ECC-native PRD-to-SRS lane instead of vague planning prose.
role: product-capability
category: meta
triggers:
  - product capability
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/product-capability/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: product-capability
---

# product-capability

## Role

Portable distillation of upstream skill `product-capability` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Translate PRD intent, roadmap asks, or product discussions into an implementation-ready capability plan that exposes constraints, invariants, interfaces, and unresolved decisions before multi-service work starts. Use when the user needs an ECC-native PRD-to-SRS lane instead of vague planning prose.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
