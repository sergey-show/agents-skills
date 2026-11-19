---
id: everything-claude-code__change-impact
name: change-impact
version: 1.0.0
description: >-
  Perform evidence-backed impact analysis before changing code, data, interfaces, or governance documents, then compare the planned impact with the actual diff after implementation. Covers call paths, data and schema, API contracts, tests, documentation, ADRs, deployment, migration, and rollback. Use for cross-module or high-risk changes, database migrations, authentication, public interfaces, blast-radius questions, pre-change checks, and post-implementation alignment.
role: change-impact
category: engineering
triggers:
  - change impact
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/change-impact/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: change-impact
---

# change-impact

## Role

Portable distillation of upstream skill `change-impact` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Perform evidence-backed impact analysis before changing code, data, interfaces, or governance documents, then compare the planned impact with the actual diff after implementation. Covers call paths, data and schema, API contracts, tests, documentation, ADRs, deployment, migration, and rollback. Use for cross-module or high-risk changes, database migrations, authentication, public interfaces, blast-radius questions, pre-change checks, and post-implementation alignment.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
