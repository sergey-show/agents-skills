---
id: everything-claude-code__api-design
name: api-design
version: 1.0.0
description: >-
  REST API design patterns including resource naming, status codes, pagination, filtering, error responses, versioning, and rate limiting for production APIs. Use when designing or reviewing REST endpoints, resource names, status codes, pagination, or versioning.
role: api-design
category: design
triggers:
  - api design
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/api-design/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: api-design
---

# api-design

## Role

Portable distillation of upstream skill `api-design` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

REST API design patterns including resource naming, status codes, pagination, filtering, error responses, versioning, and rate limiting for production APIs. Use when designing or reviewing REST endpoints, resource names, status codes, pagination, or versioning.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
