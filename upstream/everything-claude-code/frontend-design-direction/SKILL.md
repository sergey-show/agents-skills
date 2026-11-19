---
id: everything-claude-code__frontend-design-direction
name: frontend-design-direction
version: 1.0.0
description: >-
  Set an ECC-specific frontend design direction for production UI work. Use when building or improving websites, dashboards, applications, components, landing pages, visual tools, or any web UI that needs stronger product-specific design judgment.
role: frontend-design-direction
category: design
triggers:
  - frontend design direction
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/frontend-design-direction/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: frontend-design-direction
---

# frontend-design-direction

## Role

Portable distillation of upstream skill `frontend-design-direction` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Set an ECC-specific frontend design direction for production UI work. Use when building or improving websites, dashboards, applications, components, landing pages, visual tools, or any web UI that needs stronger product-specific design judgment.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
