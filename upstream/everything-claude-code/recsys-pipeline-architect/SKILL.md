---
id: everything-claude-code__recsys-pipeline-architect
name: recsys-pipeline-architect
version: 1.0.0
description: >-
  Design composable recommendation, ranking, and feed pipelines using the six-stage Source→Hydrator→Filter→Scorer→Selector→SideEffect framework popularized by xAI's open-sourced For You algorithm. Use this skill whenever the user is building any system that picks "the top K items for a (user, context)" — social feeds, content CMSs, RAG rerankers, task prioritizers, notification triage, search reranking, ad ranking.
role: recsys-pipeline-architect
category: meta
triggers:
  - recsys pipeline architect
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - search.web
  - test.run
sources:
  - research/everything-claude-code/skills/recsys-pipeline-architect/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: recsys-pipeline-architect
---

# recsys-pipeline-architect

## Role

Portable distillation of upstream skill `recsys-pipeline-architect` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design composable recommendation, ranking, and feed pipelines using the six-stage Source→Hydrator→Filter→Scorer→Selector→SideEffect framework popularized by xAI's open-sourced For You algorithm. Use this skill whenever the user is building any system that picks "the top K items for a (user, context)" — social feeds, content CMSs, RAG rerankers, task prioritizers, notification triage, search reranking, ad ranking.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
