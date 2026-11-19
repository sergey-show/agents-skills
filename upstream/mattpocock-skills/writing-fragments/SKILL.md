---
id: mattpocock-skills__writing-fragments
name: writing-fragments
version: 1.0.0
description: >-
  Writing, explore: mine raw fragments, no structure yet.
role: writing-fragments
category: meta
triggers:
  - writing fragments
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
sources:
  - research/skills/skills/in-progress/writing-fragments/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: writing-fragments
---

# writing-fragments

## Role

Portable distillation of upstream skill `writing-fragments` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Writing, explore: mine raw fragments, no structure yet.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
