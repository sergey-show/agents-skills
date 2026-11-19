---
id: everything-claude-code__mybatis-patterns
name: mybatis-patterns
version: 1.0.0
description: >-
  MyBatis and MyBatis-Spring patterns for mapper design, XML and annotation SQL, result mapping, dynamic SQL safety, transactions, batching, pagination, and query performance. Use when building or reviewing Java persistence code with MyBatis, Spring Boot, MyBatis-Spring, or MyBatis-based legacy applications.
role: mybatis-patterns
category: security
triggers:
  - mybatis patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/mybatis-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: mybatis-patterns
---

# mybatis-patterns

## Role

Portable distillation of upstream skill `mybatis-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

MyBatis and MyBatis-Spring patterns for mapper design, XML and annotation SQL, result mapping, dynamic SQL safety, transactions, batching, pagination, and query performance. Use when building or reviewing Java persistence code with MyBatis, Spring Boot, MyBatis-Spring, or MyBatis-based legacy applications.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
