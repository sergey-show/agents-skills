---
id: superpowers__dispatching-parallel-agents
name: dispatching-parallel-agents
version: 1.0.0
description: >-
  Use when facing 2+ independent tasks that can be worked on without shared state or sequential dependencies
role: dispatching-parallel-agents
category: engineering
triggers:
  - dispatching parallel agents
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - subagent.spawn
  - test.run
sources:
  - research/superpowers/skills/dispatching-parallel-agents/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: dispatching-parallel-agents
---

# dispatching-parallel-agents

## Role

Portable distillation of upstream skill `dispatching-parallel-agents` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when facing 2+ independent tasks that can be worked on without shared state or sequential dependencies

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
