---
id: everything-claude-code__springboot-tdd
name: springboot-tdd
version: 1.0.0
description: >-
  Test-driven development for Spring Boot using JUnit 5, Mockito, MockMvc, Testcontainers, and JaCoCo. Use when adding features, fixing bugs, or refactoring.
role: springboot-tdd
category: security
triggers:
  - springboot tdd
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/springboot-tdd/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: springboot-tdd
---

# springboot-tdd

## Role

Portable distillation of upstream skill `springboot-tdd` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Test-driven development for Spring Boot using JUnit 5, Mockito, MockMvc, Testcontainers, and JaCoCo. Use when adding features, fixing bugs, or refactoring.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
