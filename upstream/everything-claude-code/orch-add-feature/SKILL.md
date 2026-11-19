---
id: everything-claude-code__orch-add-feature
name: orch-add-feature
version: 1.0.0
description: >-
  Orchestrate building a brand-new feature end to end — research, plan, TDD implementation, review, and gated commit — by delegating each phase to the matching ECC agent. Use when adding a capability that does not exist yet.
role: orch-add-feature
category: research
triggers:
  - orch add feature
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/orch-add-feature/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: orch-add-feature
---

# orch-add-feature

## Role

Portable distillation of upstream skill `orch-add-feature` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Orchestrate building a brand-new feature end to end — research, plan, TDD implementation, review, and gated commit — by delegating each phase to the matching ECC agent. Use when adding a capability that does not exist yet.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
