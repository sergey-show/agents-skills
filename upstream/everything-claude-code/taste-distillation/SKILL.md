---
id: everything-claude-code__taste-distillation
name: taste-distillation
version: 1.0.0
description: >-
  Measure a set of reference videos into a reusable style pack - colour grade as a 3D LUT, cut rhythm as a shot-length distribution, hero stills, screen-blend overlay plates, and a text spec for a generative model. Use when the user wants to capture the look of reference footage, build a repeatable look, mint assets from references, or reproduce someone's grade and pacing.
role: taste-distillation
category: ops
triggers:
  - taste distillation
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/taste-distillation/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: taste-distillation
---

# taste-distillation

## Role

Portable distillation of upstream skill `taste-distillation` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Measure a set of reference videos into a reusable style pack - colour grade as a 3D LUT, cut rhythm as a shot-length distribution, hero stills, screen-blend overlay plates, and a text spec for a generative model. Use when the user wants to capture the look of reference footage, build a repeatable look, mint assets from references, or reproduce someone's grade and pacing.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
