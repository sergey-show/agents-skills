---
id: autonomous-loop
name: Autonomous Loop
version: 1.0.0
description: >-
  Designs cautious autonomous agent loops — sequential pipelines, quality cleanup passes, CI-gated PR loops, and multi-agent DAGs — with stop conditions and human gates. Use when setting up unattended or continuous agent workflows.
role: Autonomous Loop Designer
category: meta
triggers:
  - autonomous loop
  - agent loop
  - continuous agent
  - unattended agent
  - ralph loop
  - overnight agent
capabilities_required:
  - ask_user
  - filesystem.write
capabilities_optional:
  - subagent.spawn
  - shell.exec
  - git.ops
  - test.run
  - orchestrate.flow
  - memory.persist
sources:
  - research/everything-claude-code
harness: any
---

# Autonomous Loop

## Role

You design autonomous loops with explicit stop conditions, quality gates, and human approval for irreversible actions. Autonomy without brakes is a liability.

## When to use

Unattended pipelines; continuous PR loops; parallel content/code generation with merge queues; overnight agent runs.

## Workflow

1. Pick the simplest pattern that fits (sequential → CI-gated → multi-agent DAG).
2. Define per-step prompts with clear done-when; fresh context per step when possible.
3. Add a cleanup ("de-sloppify") pass after implementers.
4. Wire verify gates (tests/lint/typecheck) — fail closed.
5. Set stop rules: max iterations, spend, consecutive failures, human checkpoints.
6. Never grant unattended push/prod deploy without explicit user policy.

## Done when

Loop script/plan documented with gates, stops, and recovery; dry-run succeeded.

## See also

- [tools.md](tools.md) · [approaches.md](approaches.md) · [rules.md](rules.md)
- Related: `orchestrator`, `token-optimizer`, `eval-engineer`

## Upstream depth

- `skills/upstream/superpowers/subagent-driven-development/`
- `skills/upstream/gstack/captain/`
