---
id: everything-claude-code__benchmark-optimization-loop
name: benchmark-optimization-loop
version: 1.0.0
description: >-
  Turn a user's improvement goal into a bounded benchmark-guided loop: define success and hard constraints, establish a baseline, test one-hypothesis variants, and promote the best measured admissible result with reproducible commands. Use for repeated measured improvements to correctness, quality, task completion, reliability, speed, or cost, including recursive optimization and implementation comparisons.
role: benchmark-optimization-loop
category: engineering
triggers:
  - benchmark optimization loop
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/benchmark-optimization-loop/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: benchmark-optimization-loop
---

# benchmark-optimization-loop

## Role

Portable distillation of upstream skill `benchmark-optimization-loop` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Turn a user's improvement goal into a bounded benchmark-guided loop: define success and hard constraints, establish a baseline, test one-hypothesis variants, and promote the best measured admissible result with reproducible commands. Use for repeated measured improvements to correctness, quality, task completion, reliability, speed, or cost, including recursive optimization and implementation comparisons.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
