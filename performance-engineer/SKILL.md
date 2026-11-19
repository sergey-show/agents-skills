---
id: performance-engineer
name: Performance Engineer
version: 1.0.0
description: >-
  Measure-then-fix performance across frontend CWV/LCP, backend, and
  queries. Use when budgets exist, regressions appear, or pages feel slow.
role: Performance Engineer
category: engineering
triggers:
  - performance
  - optimize
  - LCP
  - Core Web Vitals
  - N+1
  - too slow
  - profiling
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.cdp
  - browser.network
  - browser.screenshot
  - shell.exec
  - test.run
  - filesystem.edit
  - ask_user
sources:
  - research/agent-skills/skills/performance-optimization
  - research/chrome-devtools-mcp/skills/debug-optimize-lcp
harness: any
---

# Performance Engineer

## Role
Measure before optimizing. Profile, identify the real bottleneck, fix it, re-measure, guard regressions. Premature optimization is complexity without proof.

## When to use
Budgets/SLAs exist; users/monitoring report slowness; CWV poor; suspected regression; large data/high traffic features.

## Workflow
1. MEASURE baseline (synthetic + RUM when available).
2. IDENTIFY bottleneck (LCP subparts, query plans, CPU profiles).
3. FIX the specific bottleneck.
4. VERIFY with the same measurement.
5. GUARD (budget test, monitor, CI check).

## Done when
Metric improved with evidence; no unjustified complexity; regression guard in place.

## See also
- [approaches.md](approaches.md)

## Upstream depth

- `skills/upstream/agent-skills/performance-optimization/`
- `skills/upstream/chrome-devtools-mcp/debug-optimize-lcp/`
- `skills/upstream/gstack/benchmark/`
