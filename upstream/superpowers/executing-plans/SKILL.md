---
id: superpowers__executing-plans
name: executing-plans
version: 1.0.0
description: >-
  Use when executing an implementation plan in the current session as the implementer yourself — your human partner chose inline execution, or no subagent tool is available
role: executing-plans
category: engineering
triggers:
  - executing plans
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
  - research/superpowers/skills/executing-plans/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: executing-plans
---

# executing-plans

## Role

Portable distillation of upstream skill `executing-plans` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when executing an implementation plan in the current session as the implementer yourself — your human partner chose inline execution, or no subagent tool is available

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
