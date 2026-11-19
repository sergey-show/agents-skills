---
id: everything-claude-code__orch-fix-defect
name: orch-fix-defect
version: 1.0.0
description: >-
  Orchestrate fixing a bug — reproduce it as a failing regression test, fix to green, review, and gated commit — by delegating each phase to the matching ECC agent. Use when existing behavior is broken or wrong.
role: orch-fix-defect
category: meta
triggers:
  - orch fix defect
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/orch-fix-defect/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: orch-fix-defect
---

# orch-fix-defect

## Role

Portable distillation of upstream skill `orch-fix-defect` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Orchestrate fixing a bug — reproduce it as a failing regression test, fix to green, review, and gated commit — by delegating each phase to the matching ECC agent. Use when existing behavior is broken or wrong.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
