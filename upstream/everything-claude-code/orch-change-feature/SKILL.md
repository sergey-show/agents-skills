---
id: everything-claude-code__orch-change-feature
name: orch-change-feature
version: 1.0.0
description: >-
  Orchestrate altering an existing, working feature to new desired behavior — update its tests to the new spec, change the implementation to match, review, and gated commit. Use when behavior is not broken but should be different.
role: orch-change-feature
category: meta
triggers:
  - orch change feature
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/orch-change-feature/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: orch-change-feature
---

# orch-change-feature

## Role

Portable distillation of upstream skill `orch-change-feature` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Orchestrate altering an existing, working feature to new desired behavior — update its tests to the new spec, change the implementation to match, review, and gated commit. Use when behavior is not broken but should be different.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
