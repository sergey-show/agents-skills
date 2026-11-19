---
id: mattpocock-skills__improve-codebase-architecture
name: improve-codebase-architecture
version: 1.0.0
description: >-
  Scan a codebase for deepening opportunities, present them as a visual HTML report, then grill through whichever one you pick.
role: improve-codebase-architecture
category: design
triggers:
  - improve codebase architecture
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/skills/skills/engineering/improve-codebase-architecture/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: improve-codebase-architecture
---

# improve-codebase-architecture

## Role

Portable distillation of upstream skill `improve-codebase-architecture` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Scan a codebase for deepening opportunities, present them as a visual HTML report, then grill through whichever one you pick.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
