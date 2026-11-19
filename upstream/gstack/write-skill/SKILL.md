---
id: gstack__write-skill
name: write-skill
version: 1.0.0
description: >-
  Write a new agent skill or improve one without bloat: the edit ladder, levels, drift and size checks, full diets. Use for: write a skill, improve this skill. (gstack)
role: write-skill
category: meta
triggers:
  - write skill
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/write-skill/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: write-skill
---

# write-skill

## Role

Portable distillation of upstream skill `write-skill` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Write a new agent skill or improve one without bloat: the edit ladder, levels, drift and size checks, full diets. Use for: write a skill, improve this skill. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
