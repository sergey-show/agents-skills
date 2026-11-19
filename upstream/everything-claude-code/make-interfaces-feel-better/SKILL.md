---
id: everything-claude-code__make-interfaces-feel-better
name: make-interfaces-feel-better
version: 1.0.0
description: >-
  Apply concrete design-engineering details that make interfaces feel polished. Use when reviewing or improving UI spacing, typography, borders, shadows, motion, hit areas, icons, text wrapping, and interaction states.
role: make-interfaces-feel-better
category: design
triggers:
  - make interfaces feel better
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
sources:
  - research/everything-claude-code/skills/make-interfaces-feel-better/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: make-interfaces-feel-better
---

# make-interfaces-feel-better

## Role

Portable distillation of upstream skill `make-interfaces-feel-better` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Apply concrete design-engineering details that make interfaces feel polished. Use when reviewing or improving UI spacing, typography, borders, shadows, motion, hit areas, icons, text wrapping, and interaction states.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
