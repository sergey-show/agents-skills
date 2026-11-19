---
id: agent-skills__incremental-implementation
name: incremental-implementation
version: 1.0.0
description: >-
  Delivers changes incrementally in thin, verifiable slices. Use when implementing any feature or change that touches more than one file, or when picking up the next task from a plan. Use when rolling a change out behind a feature flag, when you're about to write a large amount of code at once, or when a task feels too big to land in one step.
role: incremental-implementation
category: engineering
triggers:
  - incremental implementation
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/incremental-implementation/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: incremental-implementation
---

# incremental-implementation

## Role

Portable distillation of upstream skill `incremental-implementation` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Delivers changes incrementally in thin, verifiable slices. Use when implementing any feature or change that touches more than one file, or when picking up the next task from a plan. Use when rolling a change out behind a feature flag, when you're about to write a large amount of code at once, or when a task feels too big to land in one step.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
