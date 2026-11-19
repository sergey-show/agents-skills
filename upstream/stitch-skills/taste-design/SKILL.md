---
id: stitch-skills__taste-design
name: taste-design
version: 1.0.0
description: >-
  Semantic Design System Skill for Google Stitch. Generates agent-friendly DESIGN.md files that enforce premium, anti-generic UI standards — strict typography, calibrated color, asymmetric layouts, perpetual micro-motion, and hardware-accelerated performance.
role: taste-design
category: design
triggers:
  - taste design
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - search.web
  - test.run
sources:
  - research/stitch-skills/plugins/stitch-utilities/skills/taste-design/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: taste-design
---

# taste-design

## Role

Portable distillation of upstream skill `taste-design` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Semantic Design System Skill for Google Stitch. Generates agent-friendly DESIGN.md files that enforce premium, anti-generic UI standards — strict typography, calibrated color, asymmetric layouts, perpetual micro-motion, and hardware-accelerated performance.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
