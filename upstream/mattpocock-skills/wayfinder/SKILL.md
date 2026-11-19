---
id: mattpocock-skills__wayfinder
name: wayfinder
version: 1.0.0
description: >-
  Plan a huge chunk of work (more than one agent session can hold) as a shared map of decision tickets on your issue tracker, and resolve them one at a time until the way to the destination is clear.
role: wayfinder
category: meta
triggers:
  - wayfinder
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - subagent.spawn
  - test.run
sources:
  - research/skills/skills/engineering/wayfinder/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: wayfinder
---

# wayfinder

## Role

Portable distillation of upstream skill `wayfinder` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Plan a huge chunk of work (more than one agent session can hold) as a shared map of decision tickets on your issue tracker, and resolve them one at a time until the way to the destination is clear.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
