---
id: everything-claude-code__documentation-lookup
name: documentation-lookup
version: 1.0.0
description: >-
  Use up-to-date library and framework docs via Context7 MCP instead of training data. Activates for setup questions, API references, code examples, or when the user names a framework (e.g. React, Next.js, Prisma).
role: documentation-lookup
category: engineering
triggers:
  - documentation lookup
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/.agents/skills/documentation-lookup/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: documentation-lookup
---

# documentation-lookup

## Role

Portable distillation of upstream skill `documentation-lookup` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use up-to-date library and framework docs via Context7 MCP instead of training data. Activates for setup questions, API references, code examples, or when the user names a framework (e.g. React, Next.js, Prisma).

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
