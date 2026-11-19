---
id: everything-claude-code__blender-motion-state-inspection
name: blender-motion-state-inspection
version: 1.0.0
description: >-
  Inspects Blender characters, rigs, poses, animation retargeting, ground contact, facing direction, or model-vs-motion alignment where screenshots alone are not enough.
role: blender-motion-state-inspection
category: engineering
triggers:
  - blender motion state inspection
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
sources:
  - research/everything-claude-code/skills/blender-motion-state-inspection/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: blender-motion-state-inspection
---

# blender-motion-state-inspection

## Role

Portable distillation of upstream skill `blender-motion-state-inspection` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Inspects Blender characters, rigs, poses, animation retargeting, ground contact, facing direction, or model-vs-motion alignment where screenshots alone are not enough.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
