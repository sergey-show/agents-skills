---
id: superpowers__subagent-driven-development
name: subagent-driven-development
version: 1.0.0
description: >-
  Use when executing implementation plans with independent tasks in the current session
role: subagent-driven-development
category: engineering
triggers:
  - subagent driven development
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/superpowers/skills/subagent-driven-development/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: subagent-driven-development
---

# subagent-driven-development

## Role

Portable distillation of upstream skill `subagent-driven-development` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when executing implementation plans with independent tasks in the current session

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
