---
id: mattpocock-skills__handoff
name: handoff
version: 1.0.0
description: >-
  Compact the current conversation into a handoff document for another agent to pick up.
role: handoff
category: meta
triggers:
  - handoff
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
sources:
  - research/skills/skills/productivity/handoff/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: handoff
---

# handoff

## Role

Portable distillation of upstream skill `handoff` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Compact the current conversation into a handoff document for another agent to pick up.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
