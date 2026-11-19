---
id: everything-claude-code__accessibility
name: accessibility
version: 1.0.0
description: >-
  Design, implement, and audit accessible UI to WCAG 2.2 Level AA across Web, iOS, and Android — semantic ARIA roles and labels, accessibility traits and hints, focus management, contrast, target size, and screen-reader support. Use when building or auditing UI for accessibility compliance, keyboard navigation, or screen-reader support.
role: accessibility
category: design
triggers:
  - accessibility
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
sources:
  - research/everything-claude-code/skills/accessibility/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: accessibility
---

# accessibility

## Role

Portable distillation of upstream skill `accessibility` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design, implement, and audit accessible UI to WCAG 2.2 Level AA across Web, iOS, and Android — semantic ARIA roles and labels, accessibility traits and hints, focus management, contrast, target size, and screen-reader support. Use when building or auditing UI for accessibility compliance, keyboard navigation, or screen-reader support.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
