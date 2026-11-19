---
id: agent-skills__accessibility-engineering
name: accessibility-engineering
version: 1.0.0
description: >-
  Audits existing interfaces for WCAG 2.2 AA conformance and remediates the violations found. Use when auditing a page or component for accessibility, running axe-core or pa11y, triaging a11y violations, or checking screen reader and contrast issues before shipping.
role: accessibility-engineering
category: ops
triggers:
  - accessibility engineering
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/accessibility-engineering/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: accessibility-engineering
---

# accessibility-engineering

## Role

Portable distillation of upstream skill `accessibility-engineering` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Audits existing interfaces for WCAG 2.2 AA conformance and remediates the violations found. Use when auditing a page or component for accessibility, running axe-core or pa11y, triaging a11y violations, or checking screen reader and contrast issues before shipping.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
