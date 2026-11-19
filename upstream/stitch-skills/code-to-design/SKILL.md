---
id: stitch-skills__code-to-design
name: stitch::code-to-design
version: 1.0.0
description: >-
  Convert frontend code (Vite, React, Angular, Vue, etc.) to a Stitch Design by chaining static HTML extraction, design system extraction, and file upload. **ALWAYS** use this skill when the user's intent is to move existing web apps or React/Angular/Vue components into Stitch (e.g., requests to "save", "migrate", or "upload"). You must use this skill even for simple "save" operations, as it is the only way to ensure the design system is extracted and assets are properly linked.
role: stitch::code-to-design
category: design
triggers:
  - code to design
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
sources:
  - research/stitch-skills/plugins/stitch-design/skills/code-to-design/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: code-to-design
---

# stitch::code-to-design

## Role

Portable distillation of upstream skill `code-to-design` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Convert frontend code (Vite, React, Angular, Vue, etc.) to a Stitch Design by chaining static HTML extraction, design system extraction, and file upload. **ALWAYS** use this skill when the user's intent is to move existing web apps or React/Angular/Vue components into Stitch (e.g., requests to "save", "migrate", or "upload"). You must use this skill even for simple "save" operations, as it is the only way to ensure the design system is extracted and assets are properly linked.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
