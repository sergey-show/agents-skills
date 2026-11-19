---
id: everything-claude-code__redis-patterns
name: redis-patterns
version: 1.0.0
description: >-
  Redis data structure patterns, caching strategies, distributed locks, rate limiting, pub/sub, and connection management for production applications. Use when adding caching, a distributed lock, rate limiting, or pub/sub with Redis, or when key design needs review.
role: redis-patterns
category: meta
triggers:
  - redis patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/redis-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: redis-patterns
---

# redis-patterns

## Role

Portable distillation of upstream skill `redis-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Redis data structure patterns, caching strategies, distributed locks, rate limiting, pub/sub, and connection management for production applications. Use when adding caching, a distributed lock, rate limiting, or pub/sub with Redis, or when key design needs review.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
