---
id: mattpocock-skills__writing-shape
name: writing-shape
version: 1.0.0
description: >-
  Writing, exploit: shape raw material into an article, paragraph by paragraph.
role: writing-shape
category: engineering
triggers:
  - writing shape
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
sources:
  - research/skills/skills/in-progress/writing-shape/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: writing-shape
---

# writing-shape

## Role

Portable distillation of upstream skill `writing-shape` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Writing, exploit: shape raw material into an article, paragraph by paragraph.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
