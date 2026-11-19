---
id: everything-claude-code__manim-video
name: manim-video
version: 1.0.0
description: >-
  Build reusable Manim explainers for technical concepts, graphs, system diagrams, and product walkthroughs, then hand off to the wider ECC video stack if needed. Use when the user wants a clean animated explainer rather than a generic talking-head script.
role: manim-video
category: engineering
triggers:
  - manim video
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/manim-video/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: manim-video
---

# manim-video

## Role

Portable distillation of upstream skill `manim-video` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build reusable Manim explainers for technical concepts, graphs, system diagrams, and product walkthroughs, then hand off to the wider ECC video stack if needed. Use when the user wants a clean animated explainer rather than a generic talking-head script.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
