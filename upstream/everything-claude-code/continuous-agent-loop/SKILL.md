---
id: everything-claude-code__continuous-agent-loop
name: continuous-agent-loop
version: 1.0.0
description: >-
  Patterns for continuous autonomous agent loops with quality gates, evals, and recovery controls. Use when running an agent loop that must self-check, gate on evals, and recover from failures.
role: continuous-agent-loop
category: ops
triggers:
  - continuous agent loop
capabilities_required:
  - filesystem.read
capabilities_optional:
  - git.ops
sources:
  - research/everything-claude-code/skills/continuous-agent-loop/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: continuous-agent-loop
---

# continuous-agent-loop

## Role

Portable distillation of upstream skill `continuous-agent-loop` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Patterns for continuous autonomous agent loops with quality gates, evals, and recovery controls. Use when running an agent loop that must self-check, gate on evals, and recover from failures.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
