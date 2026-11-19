---
id: everything-claude-code__autonomous-loops
name: autonomous-loops
version: 1.0.0
description: >-
  Patterns and architectures for autonomous the coding agent loops — from simple sequential pipelines to RFC-driven multi-agent DAG systems. Retained for compatibility only: when new autonomous loop guidance is needed, use continuous-agent-loop instead.
role: autonomous-loops
category: ops
triggers:
  - autonomous loops
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/autonomous-loops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: autonomous-loops
---

# autonomous-loops

## Role

Portable distillation of upstream skill `autonomous-loops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Patterns and architectures for autonomous the coding agent loops — from simple sequential pipelines to RFC-driven multi-agent DAG systems. Retained for compatibility only: when new autonomous loop guidance is needed, use continuous-agent-loop instead.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
