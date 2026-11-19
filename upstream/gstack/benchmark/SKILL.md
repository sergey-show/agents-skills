---
id: gstack__benchmark
name: benchmark
version: 1.0.0
description: >-
  Web performance regression detection. Use for: web performance benchmark, check page speed. (gstack)
role: benchmark
category: meta
triggers:
  - benchmark
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/benchmark/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: benchmark
---

# benchmark

## Role

Portable distillation of upstream skill `benchmark` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Web performance regression detection. Use for: web performance benchmark, check page speed. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
