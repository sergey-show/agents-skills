---
id: everything-claude-code__scientific-db-pubmed-database
name: scientific-db-pubmed-database
version: 1.0.0
description: >-
  Direct PubMed and NCBI E-utilities search workflows for biomedical literature, MeSH queries, PMID lookup, citation retrieval, and API-backed literature monitoring. Use when a task needs biomedical literature from PubMed rather than general web search.
role: scientific-db-pubmed-database
category: meta
triggers:
  - scientific db pubmed database
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/scientific-db-pubmed-database/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: scientific-db-pubmed-database
---

# scientific-db-pubmed-database

## Role

Portable distillation of upstream skill `scientific-db-pubmed-database` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Direct PubMed and NCBI E-utilities search workflows for biomedical literature, MeSH queries, PMID lookup, citation retrieval, and API-backed literature monitoring. Use when a task needs biomedical literature from PubMed rather than general web search.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
