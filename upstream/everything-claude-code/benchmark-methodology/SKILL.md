---
id: everything-claude-code__benchmark-methodology
name: benchmark-methodology
version: 1.0.0
description: >-
  Use after competitive-platform-analysis has produced a tiered competitor set. Scores each competitor across nine weighted dimensions (positioning, voice, visual craft, offer packaging, evidence, enterprise-readiness, thought leadership, pricing, client's strategic tension) with explicit 1–5 rubrics and a tension-plot. Precedes competitive-report-structure.
role: benchmark-methodology
category: meta
triggers:
  - benchmark methodology
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
sources:
  - research/everything-claude-code/.agents/skills/benchmark-methodology/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: benchmark-methodology
---

# benchmark-methodology

## Role

Portable distillation of upstream skill `benchmark-methodology` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use after competitive-platform-analysis has produced a tiered competitor set. Scores each competitor across nine weighted dimensions (positioning, voice, visual craft, offer packaging, evidence, enterprise-readiness, thought leadership, pricing, client's strategic tension) with explicit 1–5 rubrics and a tension-plot. Precedes competitive-report-structure.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
