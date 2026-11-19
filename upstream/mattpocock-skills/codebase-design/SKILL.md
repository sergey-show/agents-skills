---
id: mattpocock-skills__codebase-design
name: codebase-design
version: 1.0.0
description: >-
  Shared vocabulary for designing deep modules. Use when the user wants to design or improve a module's interface, find deepening opportunities, decide where a seam goes, make code more testable or AI-navigable, or when another skill needs the deep-module vocabulary.
role: codebase-design
category: design
triggers:
  - codebase design
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/skills/skills/engineering/codebase-design/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: codebase-design
---

# codebase-design

## Role

Portable distillation of upstream skill `codebase-design` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Shared vocabulary for designing deep modules. Use when the user wants to design or improve a module's interface, find deepening opportunities, decide where a seam goes, make code more testable or AI-navigable, or when another skill needs the deep-module vocabulary.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
