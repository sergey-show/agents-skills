---
id: stitch-skills__generate-design
name: stitch::generate-design
version: 1.0.0
description: >-
  Generate new screens from text prompts or images, edit existing screens with prompts and design system tokens, and generate design variants using Stitch MCP. Includes prompt enhancement pipeline, design mappings, professional UI/UX terminology, design tokens and theme system capabilities.
role: stitch::generate-design
category: design
triggers:
  - generate design
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/stitch-skills/plugins/stitch-design/skills/generate-design/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: generate-design
---

# stitch::generate-design

## Role

Portable distillation of upstream skill `generate-design` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Generate new screens from text prompts or images, edit existing screens with prompts and design system tokens, and generate design variants using Stitch MCP. Includes prompt enhancement pipeline, design mappings, professional UI/UX terminology, design tokens and theme system capabilities.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
