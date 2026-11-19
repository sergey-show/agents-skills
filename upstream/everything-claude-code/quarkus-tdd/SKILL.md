---
id: everything-claude-code__quarkus-tdd
name: quarkus-tdd
version: 1.0.0
description: >-
  Test-driven development for Quarkus 3.x LTS using JUnit 5, Mockito, REST Assured, Camel testing, and JaCoCo. Use when adding features, fixing bugs, or refactoring event-driven services.
role: quarkus-tdd
category: security
triggers:
  - quarkus tdd
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/quarkus-tdd/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: quarkus-tdd
---

# quarkus-tdd

## Role

Portable distillation of upstream skill `quarkus-tdd` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Test-driven development for Quarkus 3.x LTS using JUnit 5, Mockito, REST Assured, Camel testing, and JaCoCo. Use when adding features, fixing bugs, or refactoring event-driven services.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
