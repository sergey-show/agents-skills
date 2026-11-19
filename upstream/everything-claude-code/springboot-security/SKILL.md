---
id: everything-claude-code__springboot-security
name: springboot-security
version: 1.0.0
description: >-
  Spring Security best practices for authn/authz, validation, CSRF, secrets, headers, rate limiting, and dependency security in Java Spring Boot services. Use when reviewing Spring Security authn/authz, validation, CSRF, secrets, headers, or rate limiting.
role: springboot-security
category: security
triggers:
  - springboot security
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
sources:
  - research/everything-claude-code/skills/springboot-security/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: springboot-security
---

# springboot-security

## Role

Portable distillation of upstream skill `springboot-security` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Spring Security best practices for authn/authz, validation, CSRF, secrets, headers, rate limiting, and dependency security in Java Spring Boot services. Use when reviewing Spring Security authn/authz, validation, CSRF, secrets, headers, or rate limiting.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
