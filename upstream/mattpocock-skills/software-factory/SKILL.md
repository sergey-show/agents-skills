---
id: mattpocock-skills__software-factory
name: software-factory
version: 1.0.0
description: >-
  Shared language for designing a software factory: the tasks it runs and the services it plugs into.
role: software-factory
category: design
triggers:
  - software factory
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - subagent.spawn
  - test.run
sources:
  - research/skills/skills/in-progress/software-factory/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: software-factory
---

# software-factory

## Role

Portable distillation of upstream skill `software-factory` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Shared language for designing a software factory: the tasks it runs and the services it plugs into.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
