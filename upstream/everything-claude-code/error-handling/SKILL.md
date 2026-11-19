---
id: everything-claude-code__error-handling
name: error-handling
version: 1.0.0
description: >-
  Patterns for robust error handling across TypeScript, Python, and Go. Covers typed errors, error boundaries, retries, circuit breakers, and user-facing error messages. Use when designing error types, retries, circuit breakers, or user-facing failure messages in TypeScript, Python, or Go.
role: error-handling
category: design
triggers:
  - error handling
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/error-handling/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: error-handling
---

# error-handling

## Role

Portable distillation of upstream skill `error-handling` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Patterns for robust error handling across TypeScript, Python, and Go. Covers typed errors, error boundaries, retries, circuit breakers, and user-facing error messages. Use when designing error types, retries, circuit breakers, or user-facing failure messages in TypeScript, Python, or Go.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
