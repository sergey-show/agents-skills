---
id: everything-claude-code__competitive-platform-analysis
name: competitive-platform-analysis
version: 1.0.0
description: >-
  Use when scoping a competitive landscape — identifying, categorising, and score-filtering a competitor set before any benchmarking begins. Decides who counts as a competitor, which tier they belong to, and which sources to mine. First step in the three-skill competitive pipeline; precedes benchmark-methodology.
role: competitive-platform-analysis
category: meta
triggers:
  - competitive platform analysis
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/competitive-platform-analysis/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: competitive-platform-analysis
---

# competitive-platform-analysis

## Role

Portable distillation of upstream skill `competitive-platform-analysis` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when scoping a competitive landscape — identifying, categorising, and score-filtering a competitor set before any benchmarking begins. Decides who counts as a competitor, which tier they belong to, and which sources to mine. First step in the three-skill competitive pipeline; precedes benchmark-methodology.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
