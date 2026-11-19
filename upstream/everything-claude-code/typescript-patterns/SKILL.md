---
id: everything-claude-code__typescript-patterns
name: typescript-patterns
version: 1.0.0
description: >-
  TypeScript patterns for strict, type-safe, maintainable code in modern TypeScript and JavaScript applications. Covers strict compiler configuration, type design, narrowing, discriminated unions, generics, async and error handling, module boundaries, dependency hygiene, and type-level testing. Use when writing or reviewing TypeScript or JavaScript code.
role: typescript-patterns
category: research
triggers:
  - typescript patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/typescript-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: typescript-patterns
---

# typescript-patterns

## Role

Portable distillation of upstream skill `typescript-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

TypeScript patterns for strict, type-safe, maintainable code in modern TypeScript and JavaScript applications. Covers strict compiler configuration, type design, narrowing, discriminated unions, generics, async and error handling, module boundaries, dependency hygiene, and type-level testing. Use when writing or reviewing TypeScript or JavaScript code.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
