---
id: stitch-skills__extract-design-md
name: stitch::extract-design-md
version: 1.0.0
description: >-
  Extract a comprehensive design system (DESIGN.md) directly from frontend source code — React, Vue, Svelte, Angular, plain HTML/CSS, or any web framework. Analyzes component files, stylesheets, Tailwind configs, theme definitions, and design tokens to produce a rich, Stitch-compatible design system document. Use this skill whenever the user wants to reverse-engineer a design system from an existing codebase, audit the visual language of a project, extract design tokens from source files, or understand the styling patterns in a frontend repo — even if they just say "what does this app look like?" or "pull out the design from this code.
role: stitch::extract-design-md
category: design
triggers:
  - extract design md
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
sources:
  - research/stitch-skills/plugins/stitch-design/skills/extract-design-md/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: extract-design-md
---

# stitch::extract-design-md

## Role

Portable distillation of upstream skill `extract-design-md` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Extract a comprehensive design system (DESIGN.md) directly from frontend source code — React, Vue, Svelte, Angular, plain HTML/CSS, or any web framework. Analyzes component files, stylesheets, Tailwind configs, theme definitions, and design tokens to produce a rich, Stitch-compatible design system document. Use this skill whenever the user wants to reverse-engineer a design system from an existing codebase, audit the visual language of a project, extract design tokens from source files, or understand the styling patterns in a frontend repo — even if they just say "what does this app look like?" or "pull out the design from this code.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
