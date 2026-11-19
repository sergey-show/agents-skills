---
id: everything-claude-code__rust-patterns
name: rust-patterns
version: 1.0.0
description: >-
  Idiomatic Rust patterns, ownership, error handling, traits, concurrency, and best practices for building safe, performant applications. Use when writing or reviewing Rust code and ownership, error handling, traits, or concurrency is in question.
role: rust-patterns
category: design
triggers:
  - rust patterns
capabilities_required:
  - filesystem.read
capabilities_optional:
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/rust-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: rust-patterns
---

# rust-patterns

## Role

Portable distillation of upstream skill `rust-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Idiomatic Rust patterns, ownership, error handling, traits, concurrency, and best practices for building safe, performant applications. Use when writing or reviewing Rust code and ownership, error handling, traits, or concurrency is in question.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
