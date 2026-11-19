---
id: everything-claude-code__orch-build-mvp
name: orch-build-mvp
version: 1.0.0
description: >-
  Orchestrate bootstrapping a working MVP from a design or spec document — ingest the SDD/PRD, plan thin vertical slices, scaffold the first end-to-end slice, then drive a generator-evaluator build loop with review and gated feat commits. Use when a design or spec document must become a running MVP through planned vertical slices.
role: orch-build-mvp
category: design
triggers:
  - orch build mvp
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/orch-build-mvp/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: orch-build-mvp
---

# orch-build-mvp

## Role

Portable distillation of upstream skill `orch-build-mvp` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Orchestrate bootstrapping a working MVP from a design or spec document — ingest the SDD/PRD, plan thin vertical slices, scaffold the first end-to-end slice, then drive a generator-evaluator build loop with review and gated feat commits. Use when a design or spec document must become a running MVP through planned vertical slices.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
