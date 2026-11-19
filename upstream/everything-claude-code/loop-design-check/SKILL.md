---
id: everything-claude-code__loop-design-check
name: loop-design-check
version: 1.0.0
description: >-
  Design a goal-oriented agent loop or review one for failure modes: spinning, Goodhart-gaming the verifier, or running a wrong answer to completion. Covers machine-decidable goals, loop types, plan/build/judge skeletons, and runaway prevention; mechanism wiring lives in autonomous-loops. Use when designing, writing, or checking an agent loop. 中文触发：写 loop、设计 loop、做一个 loop、检查 loop 对不对、loop 体检、loop 会不会跑飞、可判定目标、五个崩法、plan build judge。
role: loop-design-check
category: design
triggers:
  - loop design check
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
  - research/everything-claude-code/skills/loop-design-check/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: loop-design-check
---

# loop-design-check

## Role

Portable distillation of upstream skill `loop-design-check` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design a goal-oriented agent loop or review one for failure modes: spinning, Goodhart-gaming the verifier, or running a wrong answer to completion. Covers machine-decidable goals, loop types, plan/build/judge skeletons, and runaway prevention; mechanism wiring lives in autonomous-loops. Use when designing, writing, or checking an agent loop. 中文触发：写 loop、设计 loop、做一个 loop、检查 loop 对不对、loop 体检、loop 会不会跑飞、可判定目标、五个崩法、plan build judge。

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
