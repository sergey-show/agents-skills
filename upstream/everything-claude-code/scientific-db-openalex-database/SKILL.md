---
id: everything-claude-code__scientific-db-openalex-database
name: scientific-db-openalex-database
version: 1.0.0
description: >-
  OpenAlex REST API workflows for cross-disciplinary literature search, DOI/PMID lookup, open-access links, citation counts, and reproducible search logs. Use when a task needs scholarly works from every field (not only biomedicine), or needs to resolve a DOI, PMID or OpenAlex ID to full metadata.
role: scientific-db-openalex-database
category: meta
triggers:
  - scientific db openalex database
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
sources:
  - research/everything-claude-code/skills/scientific-db-openalex-database/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: scientific-db-openalex-database
---

# scientific-db-openalex-database

## Role

Portable distillation of upstream skill `scientific-db-openalex-database` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

OpenAlex REST API workflows for cross-disciplinary literature search, DOI/PMID lookup, open-access links, citation counts, and reproducible search logs. Use when a task needs scholarly works from every field (not only biomedicine), or needs to resolve a DOI, PMID or OpenAlex ID to full metadata.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
