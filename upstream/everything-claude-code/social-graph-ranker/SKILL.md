---
id: everything-claude-code__social-graph-ranker
name: social-graph-ranker
version: 1.0.0
description: >-
  Weighted social-graph ranking for warm intro discovery, bridge scoring, and network gap analysis across X and LinkedIn. Use when the user wants the reusable graph-ranking engine itself, not the broader outreach or network-maintenance workflow layered on top of it.
role: social-graph-ranker
category: research
triggers:
  - social graph ranker
capabilities_required:
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/social-graph-ranker/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: social-graph-ranker
---

# social-graph-ranker

## Role

Portable distillation of upstream skill `social-graph-ranker` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Weighted social-graph ranking for warm intro discovery, bridge scoring, and network gap analysis across X and LinkedIn. Use when the user wants the reusable graph-ranking engine itself, not the broader outreach or network-maintenance workflow layered on top of it.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
