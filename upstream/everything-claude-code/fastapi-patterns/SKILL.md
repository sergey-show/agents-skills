---
id: everything-claude-code__fastapi-patterns
name: fastapi-patterns
version: 1.0.0
description: >-
  FastAPI best practices covering project structure, Pydantic v2 schemas, dependency injection, async handlers, authentication, authorization, transactional service layers, and testing with httpx and pytest. Use when building or reviewing FastAPI apps — Pydantic schemas, dependencies, async handlers, auth, or tests.
role: fastapi-patterns
category: engineering
triggers:
  - fastapi patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/fastapi-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: fastapi-patterns
---

# fastapi-patterns

## Role

Portable distillation of upstream skill `fastapi-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

FastAPI best practices covering project structure, Pydantic v2 schemas, dependency injection, async handlers, authentication, authorization, transactional service layers, and testing with httpx and pytest. Use when building or reviewing FastAPI apps — Pydantic schemas, dependencies, async handlers, auth, or tests.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
