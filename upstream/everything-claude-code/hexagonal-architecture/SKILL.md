---
id: everything-claude-code__hexagonal-architecture
name: hexagonal-architecture
version: 1.0.0
description: >-
  Design, implement, and refactor Ports & Adapters systems with clear domain boundaries, dependency inversion, and testable use-case orchestration across TypeScript, Java, Kotlin, and Go services. Use when introducing or refactoring toward Ports and Adapters, or when domain logic has become entangled with I/O.
role: hexagonal-architecture
category: engineering
triggers:
  - hexagonal architecture
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/hexagonal-architecture/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: hexagonal-architecture
---

# hexagonal-architecture

## Role

Portable distillation of upstream skill `hexagonal-architecture` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design, implement, and refactor Ports & Adapters systems with clear domain boundaries, dependency inversion, and testable use-case orchestration across TypeScript, Java, Kotlin, and Go services. Use when introducing or refactoring toward Ports and Adapters, or when domain logic has become entangled with I/O.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
