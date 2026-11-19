---
id: mattpocock-skills__loop-me
name: loop-me
version: 1.0.0
description: >-
  Grill me about specs for the workflows I want to build, within this workspace.
role: loop-me
category: engineering
triggers:
  - loop me
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/skills/skills/in-progress/loop-me/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: loop-me
---

# loop-me

## Role

Portable distillation of upstream skill `loop-me` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Grill me about specs for the workflows I want to build, within this workspace.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
