---
id: everything-claude-code__csharp-testing
name: csharp-testing
version: 1.0.0
description: >-
  C# and .NET testing patterns with xUnit, FluentAssertions, mocking, integration tests, and test organization best practices. Use when writing or reviewing xUnit tests, mocks, or integration tests in a C# / .NET project.
role: csharp-testing
category: engineering
triggers:
  - csharp testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/csharp-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: csharp-testing
---

# csharp-testing

## Role

Portable distillation of upstream skill `csharp-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

C# and .NET testing patterns with xUnit, FluentAssertions, mocking, integration tests, and test organization best practices. Use when writing or reviewing xUnit tests, mocks, or integration tests in a C# / .NET project.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
