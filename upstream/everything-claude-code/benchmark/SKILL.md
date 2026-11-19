---
id: everything-claude-code__benchmark
name: benchmark
version: 1.0.0
description: >-
  Measure performance baselines and detect regressions across browser Core Web Vitals (LCP, INP, CLS, page weight), API endpoint latency percentiles, and build/test feedback times, with before/after comparison stored in git-tracked .ecc/benchmarks JSON. Use when checking page speed, responding to 'it feels slow' reports, verifying launch performance targets, or comparing stack alternatives.
role: benchmark
category: engineering
triggers:
  - benchmark
capabilities_required:
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/benchmark/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: benchmark
---

# benchmark

## Role

Portable distillation of upstream skill `benchmark` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Measure performance baselines and detect regressions across browser Core Web Vitals (LCP, INP, CLS, page weight), API endpoint latency percentiles, and build/test feedback times, with before/after comparison stored in git-tracked .ecc/benchmarks JSON. Use when checking page speed, responding to 'it feels slow' reports, verifying launch performance targets, or comparing stack alternatives.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
