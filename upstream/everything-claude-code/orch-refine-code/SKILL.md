---
id: everything-claude-code__orch-refine-code
name: orch-refine-code
version: 1.0.0
description: >-
  Orchestrate a behavior-preserving refactor — confirm tests are green, restructure without changing behavior, keep tests green, review, and gated commit. Use when the structure should improve but behavior must not change.
role: orch-refine-code
category: meta
triggers:
  - orch refine code
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/orch-refine-code/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: orch-refine-code
---

# orch-refine-code

## Role

Portable distillation of upstream skill `orch-refine-code` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Orchestrate a behavior-preserving refactor — confirm tests are green, restructure without changing behavior, keep tests green, review, and gated commit. Use when the structure should improve but behavior must not change.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
