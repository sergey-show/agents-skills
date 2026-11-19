---
id: agent-skills__deprecation-and-migration
name: deprecation-and-migration
version: 1.0.0
description: >-
  Manages deprecation and migration. Use when removing old systems, APIs, or features. Use when migrating users from one implementation to another. Use when migrating a database schema in production, such as renaming or dropping a column without downtime (expand/contract). Use when deciding whether to maintain or sunset existing code.
role: deprecation-and-migration
category: security
triggers:
  - deprecation and migration
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/agent-skills/skills/deprecation-and-migration/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: deprecation-and-migration
---

# deprecation-and-migration

## Role

Portable distillation of upstream skill `deprecation-and-migration` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Manages deprecation and migration. Use when removing old systems, APIs, or features. Use when migrating users from one implementation to another. Use when migrating a database schema in production, such as renaming or dropping a column without downtime (expand/contract). Use when deciding whether to maintain or sunset existing code.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
