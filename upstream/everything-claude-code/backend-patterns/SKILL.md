---
id: everything-claude-code__backend-patterns
name: backend-patterns
version: 1.0.0
description: >-
  Backend architecture patterns, API design, database optimization, and server-side best practices for Node.js, Express, and Next.js API routes. Use when building or reviewing Node.js, Express, or Next.js API routes and their data access.
role: backend-patterns
category: design
triggers:
  - backend patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  []
sources:
  - research/everything-claude-code/.agents/skills/backend-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: backend-patterns
---

# backend-patterns

## Role

Portable distillation of upstream skill `backend-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Backend architecture patterns, API design, database optimization, and server-side best practices for Node.js, Express, and Next.js API routes. Use when building or reviewing Node.js, Express, or Next.js API routes and their data access.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
