---
id: everything-claude-code__fsharp-testing
name: fsharp-testing
version: 1.0.0
description: >-
  F# testing patterns with xUnit, FsUnit, Unquote, FsCheck property-based testing, integration tests, and test organization best practices. Use when writing F# tests with xUnit, FsUnit, Unquote, or FsCheck.
role: fsharp-testing
category: engineering
triggers:
  - fsharp testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/fsharp-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: fsharp-testing
---

# fsharp-testing

## Role

Portable distillation of upstream skill `fsharp-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

F# testing patterns with xUnit, FsUnit, Unquote, FsCheck property-based testing, integration tests, and test organization best practices. Use when writing F# tests with xUnit, FsUnit, Unquote, or FsCheck.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
