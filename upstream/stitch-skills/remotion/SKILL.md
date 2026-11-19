---
id: stitch-skills__remotion
name: remotion
version: 1.0.0
description: >-
  Generate walkthrough videos from Stitch projects using Remotion with smooth transitions, zooming, and text overlays
role: remotion
category: design
triggers:
  - remotion
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - test.run
sources:
  - research/stitch-skills/plugins/stitch-build/skills/remotion/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: remotion
---

# remotion

## Role

Portable distillation of upstream skill `remotion` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Generate walkthrough videos from Stitch projects using Remotion with smooth transitions, zooming, and text overlays

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
