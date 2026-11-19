---
id: superpowers__writing-skills
name: writing-skills
version: 1.0.0
description: >-
  Use when creating new skills, editing existing skills, or verifying skills work before deployment
role: writing-skills
category: meta
triggers:
  - writing skills
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/superpowers/skills/writing-skills/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: writing-skills
---

# writing-skills

## Role

Portable distillation of upstream skill `writing-skills` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when creating new skills, editing existing skills, or verifying skills work before deployment

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
