---
id: mattpocock-skills__wait-what
name: wait-what
version: 1.0.0
description: >-
  Stop. That last message did not land: re-pitch it.
role: wait-what
category: engineering
triggers:
  - wait what
capabilities_required:
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/skills/skills/productivity/wait-what/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: wait-what
---

# wait-what

## Role

Portable distillation of upstream skill `wait-what` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Stop. That last message did not land: re-pitch it.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
