---
id: everything-claude-code__design-system
name: design-system
version: 1.0.0
description: >-
  Generate a design system from an existing codebase or audit one for visual consistency: extract tokens (colors, typography, spacing, shadows) into design-tokens.json and CSS custom properties with DESIGN.md rationale and an interactive HTML preview, score the UI across 10 dimensions, and flag AI-slop patterns. Use when starting a design system, auditing visual consistency before a redesign, or reviewing a PR that touches styling.
role: design-system
category: design
triggers:
  - design system
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
sources:
  - research/everything-claude-code/skills/design-system/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: design-system
---

# design-system

## Role

Portable distillation of upstream skill `design-system` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Generate a design system from an existing codebase or audit one for visual consistency: extract tokens (colors, typography, spacing, shadows) into design-tokens.json and CSS custom properties with DESIGN.md rationale and an interactive HTML preview, score the UI across 10 dimensions, and flag AI-slop patterns. Use when starting a design system, auditing visual consistency before a redesign, or reviewing a PR that touches styling.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
