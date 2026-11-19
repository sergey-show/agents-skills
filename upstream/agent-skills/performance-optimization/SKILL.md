---
id: agent-skills__performance-optimization
name: performance-optimization
version: 1.0.0
description: >-
  Optimizes application performance across frontend, backend, queries, and databases. Use when performance requirements exist, when you suspect performance regressions, when Core Web Vitals or load times need improvement, when N+1 query patterns need fixing, or when profiling reveals bottlenecks.
role: performance-optimization
category: engineering
triggers:
  - performance optimization
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
  - research/agent-skills/skills/performance-optimization/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: performance-optimization
---

# performance-optimization

## Role

Portable distillation of upstream skill `performance-optimization` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Optimizes application performance across frontend, backend, queries, and databases. Use when performance requirements exist, when you suspect performance regressions, when Core Web Vitals or load times need improvement, when N+1 query patterns need fixing, or when profiling reveals bottlenecks.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
