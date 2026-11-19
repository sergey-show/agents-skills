---
id: everything-claude-code__quarkus-security
name: quarkus-security
version: 1.0.0
description: >-
  Quarkus security implementation patterns: JWT and OIDC authentication, @RolesAllowed RBAC and SecurityIdentity checks, Bean Validation and custom validators, parameterized Panache queries, BCrypt password hashing, CORS and security headers, rate limiting, audit logging, Vault or environment-variable secrets, and dependency CVE scanning. Use when adding authentication or authorization, validating input, managing secrets, or hardening a Quarkus application.
role: quarkus-security
category: security
triggers:
  - quarkus security
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/quarkus-security/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: quarkus-security
---

# quarkus-security

## Role

Portable distillation of upstream skill `quarkus-security` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Quarkus security implementation patterns: JWT and OIDC authentication, @RolesAllowed RBAC and SecurityIdentity checks, Bean Validation and custom validators, parameterized Panache queries, BCrypt password hashing, CORS and security headers, rate limiting, audit logging, Vault or environment-variable secrets, and dependency CVE scanning. Use when adding authentication or authorization, validating input, managing secrets, or hardening a Quarkus application.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
