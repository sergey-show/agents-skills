---
id: everything-claude-code__frontend-a11y
name: frontend-a11y
version: 1.0.0
description: >-
  Accessibility patterns for React and Next.js — semantic HTML, ARIA attributes, form labeling, keyboard navigation, focus management, and screen reader support. Use when building or reviewing forms, modals, dropdowns, tooltips, or tabs, fixing a11y lint or code-review findings, or wiring up keyboard navigation and focus management.
role: frontend-a11y
category: engineering
triggers:
  - frontend a11y
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
sources:
  - research/everything-claude-code/skills/frontend-a11y/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: frontend-a11y
---

# frontend-a11y

## Role

Portable distillation of upstream skill `frontend-a11y` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Accessibility patterns for React and Next.js — semantic HTML, ARIA attributes, form labeling, keyboard navigation, focus management, and screen reader support. Use when building or reviewing forms, modals, dropdowns, tooltips, or tabs, fixing a11y lint or code-review findings, or wiring up keyboard navigation and focus management.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
