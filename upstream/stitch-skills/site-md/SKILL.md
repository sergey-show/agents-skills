---
id: stitch-skills__site-md
name: site-md
version: 1.0.0
description: >-
  Analyze a project description or site requirements and synthesize a project constitution into SITE.md for the Stitch Build Loop
role: site-md
category: design
triggers:
  - site md
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/stitch-skills/plugins/stitch-utilities/skills/site-md/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: site-md
---

# site-md

## Role

Portable distillation of upstream skill `site-md` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Analyze a project description or site requirements and synthesize a project constitution into SITE.md for the Stitch Build Loop

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
