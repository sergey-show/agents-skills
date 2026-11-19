---
id: everything-claude-code__competitive-report-structure
name: competitive-report-structure
version: 1.0.0
description: >-
  Use after benchmark-methodology has produced scored competitor profile cards. Assembles findings into a decision-grade report: landscape map, competitor profiles, benchmarking matrix, white-space analysis, strategic recommendations, and team alignment trigger questions. Final step in the three-skill competitive pipeline.
role: competitive-report-structure
category: meta
triggers:
  - competitive report structure
capabilities_required:
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/.agents/skills/competitive-report-structure/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: competitive-report-structure
---

# competitive-report-structure

## Role

Portable distillation of upstream skill `competitive-report-structure` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use after benchmark-methodology has produced scored competitor profile cards. Assembles findings into a decision-grade report: landscape map, competitor profiles, benchmarking matrix, white-space analysis, strategic recommendations, and team alignment trigger questions. Final step in the three-skill competitive pipeline.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
