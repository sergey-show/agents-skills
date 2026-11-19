---
id: rea__rea-analysis-optimization
name: rea-analysis-optimization
version: 1.0.0
description: >-
  Optimize REA providers and shared analysis workflows for agent context, latency, CPU, and memory while preserving correctness and Evidence. Use for analysis bottlenecks and cache or query design; CI/test-suite optimization belongs to rea-ci-tests-audit.
role: rea-analysis-optimization
category: design
triggers:
  - rea analysis optimization
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/rea/.agents/skills/rea-analysis-optimization/SKILL.md
harness: any
upstream_repo: rea
upstream_skill: rea-analysis-optimization
---

# rea-analysis-optimization

## Role

Portable distillation of upstream skill `rea-analysis-optimization` from `rea`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Optimize REA providers and shared analysis workflows for agent context, latency, CPU, and memory while preserving correctness and Evidence. Use for analysis bottlenecks and cache or query design; CI/test-suite optimization belongs to rea-ci-tests-audit.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
