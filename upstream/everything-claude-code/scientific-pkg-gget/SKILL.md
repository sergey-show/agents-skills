---
id: everything-claude-code__scientific-pkg-gget
name: scientific-pkg-gget
version: 1.0.0
description: >-
  gget CLI and Python workflow for quick genomic database queries, sequence lookup, BLAST-style searches, enrichment checks, and reproducible bioinformatics evidence logs. Use when a task needs quick bioinformatics lookup across genomic reference databases with the gget CLI or Python package.
role: scientific-pkg-gget
category: meta
triggers:
  - scientific pkg gget
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/scientific-pkg-gget/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: scientific-pkg-gget
---

# scientific-pkg-gget

## Role

Portable distillation of upstream skill `scientific-pkg-gget` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

gget CLI and Python workflow for quick genomic database queries, sequence lookup, BLAST-style searches, enrichment checks, and reproducible bioinformatics evidence logs. Use when a task needs quick bioinformatics lookup across genomic reference databases with the gget CLI or Python package.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
