---
id: everything-claude-code__customs-trade-compliance
name: customs-trade-compliance
version: 1.0.0
description: >-
  Codified customs and trade compliance expertise — HS/HTS tariff classification with GRI rules, commercial invoices and entry documentation, Incoterms 2020, FTA qualification and duty optimization (USMCA, RCEP, FTZs, drawback), denied-party screening, and penalty mitigation across US, EU, UK, and APAC jurisdictions. Use when classifying goods, preparing import/export documentation, screening restricted parties, responding to customs audits or CF-28/penalty notices, or optimizing duties.
role: customs-trade-compliance
category: engineering
triggers:
  - customs trade compliance
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/customs-trade-compliance/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: customs-trade-compliance
---

# customs-trade-compliance

## Role

Portable distillation of upstream skill `customs-trade-compliance` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Codified customs and trade compliance expertise — HS/HTS tariff classification with GRI rules, commercial invoices and entry documentation, Incoterms 2020, FTA qualification and duty optimization (USMCA, RCEP, FTZs, drawback), denied-party screening, and penalty mitigation across US, EU, UK, and APAC jurisdictions. Use when classifying goods, preparing import/export documentation, screening restricted parties, responding to customs audits or CF-28/penalty notices, or optimizing duties.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
