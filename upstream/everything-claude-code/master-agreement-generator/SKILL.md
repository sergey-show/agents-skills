---
id: everything-claude-code__master-agreement-generator
name: master-agreement-generator
version: 1.0.0
description: >-
  Generate review drafts of counterparty master agreements from one template plus a JSON spec, with role-selected clauses and a Schedule A workflow limited to the executed agreement's notice authority. Use when you need reproducible drafting and separately reviewed execution preparation.
role: master-agreement-generator
category: design
triggers:
  - master agreement generator
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/master-agreement-generator/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: master-agreement-generator
---

# master-agreement-generator

## Role

Portable distillation of upstream skill `master-agreement-generator` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Generate review drafts of counterparty master agreements from one template plus a JSON spec, with role-selected clauses and a Schedule A workflow limited to the executed agreement's notice authority. Use when you need reproducible drafting and separately reviewed execution preparation.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
