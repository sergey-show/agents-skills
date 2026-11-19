---
id: mattpocock-skills__to-questionnaire
name: to-questionnaire
version: 1.0.0
description: >-
  Turn a decision you can't fully answer into a questionnaire for someone else to fill in.
role: to-questionnaire
category: engineering
triggers:
  - to questionnaire
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/skills/skills/productivity/to-questionnaire/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: to-questionnaire
---

# to-questionnaire

## Role

Portable distillation of upstream skill `to-questionnaire` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Turn a decision you can't fully answer into a questionnaire for someone else to fill in.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
