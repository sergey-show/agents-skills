---
id: everything-claude-code__dotnet-patterns
name: dotnet-patterns
version: 1.0.0
description: >-
  Idiomatic C# and .NET patterns, conventions, dependency injection, async/await, and best practices for building robust, maintainable .NET applications. Use when writing or reviewing C# / .NET code — DI, async, or general conventions.
role: dotnet-patterns
category: design
triggers:
  - dotnet patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/dotnet-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: dotnet-patterns
---

# dotnet-patterns

## Role

Portable distillation of upstream skill `dotnet-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Idiomatic C# and .NET patterns, conventions, dependency injection, async/await, and best practices for building robust, maintainable .NET applications. Use when writing or reviewing C# / .NET code — DI, async, or general conventions.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
