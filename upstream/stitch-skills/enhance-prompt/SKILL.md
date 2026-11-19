---
id: stitch-skills__enhance-prompt
name: enhance-prompt
version: 1.0.0
description: >-
  Transforms vague UI ideas into polished, Stitch-optimized prompts. Enhances specificity, adds UI/UX keywords, injects design system context, and structures output for better generation results.
role: enhance-prompt
category: design
triggers:
  - enhance prompt
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - test.run
sources:
  - research/stitch-skills/plugins/stitch-utilities/skills/enhance-prompt/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: enhance-prompt
---

# enhance-prompt

## Role

Portable distillation of upstream skill `enhance-prompt` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Transforms vague UI ideas into polished, Stitch-optimized prompts. Enhances specificity, adds UI/UX keywords, injects design system context, and structures output for better generation results.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
