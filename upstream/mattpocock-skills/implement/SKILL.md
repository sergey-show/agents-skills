---
id: mattpocock-skills__implement
name: implement
version: 1.0.0
description: >-
  Implement a piece of work based on a spec or set of tickets.
role: implement
category: meta
triggers:
  - implement
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/skills/skills/engineering/implement/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: implement
---

# implement

## Role

Portable distillation of upstream skill `implement` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Implement a piece of work based on a spec or set of tickets.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
