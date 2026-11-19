---
id: everything-claude-code__brownfield-retrospective
name: brownfield-retrospective
version: 1.0.0
description: >-
  Run the ECC engineering process retroactively against an existing project slice. Audit current state, reconstruct past decisions, produce a four-axis gap register (thinking, coding practice, missing features, technology selection), then execute fixes forward through the plan-TDD-review pipeline. Use when adopting ECC mid-project, taking over an inherited codebase, or asking what was missed and what would have been built differently from day one.
role: brownfield-retrospective
category: engineering
triggers:
  - brownfield retrospective
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/brownfield-retrospective/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: brownfield-retrospective
---

# brownfield-retrospective

## Role

Portable distillation of upstream skill `brownfield-retrospective` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Run the ECC engineering process retroactively against an existing project slice. Audit current state, reconstruct past decisions, produce a four-axis gap register (thinking, coding practice, missing features, technology selection), then execute fixes forward through the plan-TDD-review pipeline. Use when adopting ECC mid-project, taking over an inherited codebase, or asking what was missed and what would have been built differently from day one.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
