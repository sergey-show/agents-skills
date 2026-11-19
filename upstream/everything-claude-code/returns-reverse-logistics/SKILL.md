---
id: everything-claude-code__returns-reverse-logistics
name: returns-reverse-logistics
version: 1.0.0
description: >-
  Codified expertise for returns authorization, receipt and inspection, disposition decisions, refund processing, fraud detection, and warranty claims management. Informed by returns operations managers with 15+ years experience. Includes grading frameworks, disposition economics, fraud pattern recognition, and vendor recovery processes. Use when handling product returns, reverse logistics, refund decisions, return fraud detection, or warranty claims.
role: returns-reverse-logistics
category: research
triggers:
  - returns reverse logistics
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - test.run
sources:
  - research/everything-claude-code/skills/returns-reverse-logistics/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: returns-reverse-logistics
---

# returns-reverse-logistics

## Role

Portable distillation of upstream skill `returns-reverse-logistics` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Codified expertise for returns authorization, receipt and inspection, disposition decisions, refund processing, fraud detection, and warranty claims management. Informed by returns operations managers with 15+ years experience. Includes grading frameworks, disposition economics, fraud pattern recognition, and vendor recovery processes. Use when handling product returns, reverse logistics, refund decisions, return fraud detection, or warranty claims.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
