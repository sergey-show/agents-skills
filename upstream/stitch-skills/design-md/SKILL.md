---
id: stitch-skills__design-md
name: design-md
version: 1.0.0
description: >-
  Analyze Stitch projects and synthesize a semantic design system into DESIGN.md files
role: design-md
category: design
triggers:
  - design md
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
sources:
  - research/stitch-skills/plugins/stitch-utilities/skills/design-md/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: design-md
---

# design-md

## Role

Portable distillation of upstream skill `design-md` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Analyze Stitch projects and synthesize a semantic design system into DESIGN.md files

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
