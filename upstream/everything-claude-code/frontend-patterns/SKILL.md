---
id: everything-claude-code__frontend-patterns
name: frontend-patterns
version: 1.0.0
description: >-
  Frontend development patterns for React, Next.js, state management, performance optimization, and UI best practices. Use when building or reviewing React or Next.js components, state, or render performance.
role: frontend-patterns
category: engineering
triggers:
  - frontend patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/frontend-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: frontend-patterns
---

# frontend-patterns

## Role

Portable distillation of upstream skill `frontend-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Frontend development patterns for React, Next.js, state management, performance optimization, and UI best practices. Use when building or reviewing React or Next.js components, state, or render performance.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
