---
id: everything-claude-code__rust-testing
name: rust-testing
version: 1.0.0
description: >-
  Rust testing patterns including unit tests, integration tests, async testing, property-based testing, mocking, and coverage. Follows TDD methodology. Use when writing Rust tests — unit, integration, async, property-based, or coverage.
role: rust-testing
category: engineering
triggers:
  - rust testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/rust-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: rust-testing
---

# rust-testing

## Role

Portable distillation of upstream skill `rust-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Rust testing patterns including unit tests, integration tests, async testing, property-based testing, mocking, and coverage. Follows TDD methodology. Use when writing Rust tests — unit, integration, async, property-based, or coverage.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
