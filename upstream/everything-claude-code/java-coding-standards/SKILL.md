---
id: everything-claude-code__java-coding-standards
name: java-coding-standards
version: 1.0.0
description: >-
  Java coding standards for Spring Boot and Quarkus services: naming, immutability, Optional usage, streams, exceptions, generics, CDI, reactive patterns, and project layout. Automatically applies framework-specific conventions. Use when writing or reviewing Java in a Spring Boot or Quarkus service.
role: java-coding-standards
category: engineering
triggers:
  - java coding standards
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/java-coding-standards/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: java-coding-standards
---

# java-coding-standards

## Role

Portable distillation of upstream skill `java-coding-standards` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Java coding standards for Spring Boot and Quarkus services: naming, immutability, Optional usage, streams, exceptions, generics, CDI, reactive patterns, and project layout. Automatically applies framework-specific conventions. Use when writing or reviewing Java in a Spring Boot or Quarkus service.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
