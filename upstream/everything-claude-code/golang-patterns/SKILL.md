---
id: everything-claude-code__golang-patterns
name: golang-patterns
version: 1.0.0
description: >-
  Idiomatic Go patterns, best practices, and conventions for building robust, efficient, and maintainable Go applications. Use when writing or reviewing Go code and idiomatic structure or conventions are in question.
role: golang-patterns
category: design
triggers:
  - golang patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/golang-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: golang-patterns
---

# golang-patterns

## Role

Portable distillation of upstream skill `golang-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Idiomatic Go patterns, best practices, and conventions for building robust, efficient, and maintainable Go applications. Use when writing or reviewing Go code and idiomatic structure or conventions are in question.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
