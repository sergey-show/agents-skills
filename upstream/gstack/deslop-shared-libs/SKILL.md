---
id: gstack__deslop-shared-libs
name: deslop-shared-libs
version: 1.0.0
description: >-
  Find worthwhile shared-code extractions in recent work. Use for: find code worth sharing. (gstack)
role: deslop-shared-libs
category: meta
triggers:
  - deslop shared libs
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/deslop-shared-libs/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: deslop-shared-libs
---

# deslop-shared-libs

## Role

Portable distillation of upstream skill `deslop-shared-libs` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Find worthwhile shared-code extractions in recent work. Use for: find code worth sharing. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
