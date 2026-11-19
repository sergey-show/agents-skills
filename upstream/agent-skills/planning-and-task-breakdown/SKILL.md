---
id: agent-skills__planning-and-task-breakdown
name: planning-and-task-breakdown
version: 1.0.0
description: >-
  Breaks work into ordered tasks. Use when you have a spec or clear requirements and need to break work into implementable tasks. Use when a task feels too large to start, when you need to estimate scope, or when parallel work is possible.
role: planning-and-task-breakdown
category: engineering
triggers:
  - planning and task breakdown
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/planning-and-task-breakdown/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: planning-and-task-breakdown
---

# planning-and-task-breakdown

## Role

Portable distillation of upstream skill `planning-and-task-breakdown` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Breaks work into ordered tasks. Use when you have a spec or clear requirements and need to break work into implementable tasks. Use when a task feels too large to start, when you need to estimate scope, or when parallel work is possible.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
