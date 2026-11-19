---
id: everything-claude-code__architecture-decision-records
name: architecture-decision-records
version: 1.0.0
description: >-
  Capture architectural decisions as numbered ADR markdown files in docs/adr/ with context, alternatives considered, consequences, and an index README. Use when the user says 'record this decision' or 'ADR this', chooses between frameworks or databases, discusses trade-offs, or asks why the codebase is shaped this way.
role: architecture-decision-records
category: design
triggers:
  - architecture decision records
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/architecture-decision-records/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: architecture-decision-records
---

# architecture-decision-records

## Role

Portable distillation of upstream skill `architecture-decision-records` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Capture architectural decisions as numbered ADR markdown files in docs/adr/ with context, alternatives considered, consequences, and an index README. Use when the user says 'record this decision' or 'ADR this', chooses between frameworks or databases, discusses trade-offs, or asks why the codebase is shaped this way.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
