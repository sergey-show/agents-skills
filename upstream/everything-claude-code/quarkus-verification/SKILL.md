---
id: everything-claude-code__quarkus-verification
name: quarkus-verification
version: 1.0.0
description: >-
  Verification loop for Quarkus projects: build, static analysis (Checkstyle, PMD, SpotBugs), tests with JaCoCo coverage, OWASP dependency and container security scans, GraalVM native compilation, health checks, and config validation. Use when verifying a Quarkus service before a PR, after major refactoring or dependency upgrades, or pre-deploy.
role: quarkus-verification
category: security
triggers:
  - quarkus verification
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/quarkus-verification/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: quarkus-verification
---

# quarkus-verification

## Role

Portable distillation of upstream skill `quarkus-verification` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Verification loop for Quarkus projects: build, static analysis (Checkstyle, PMD, SpotBugs), tests with JaCoCo coverage, OWASP dependency and container security scans, GraalVM native compilation, health checks, and config validation. Use when verifying a Quarkus service before a PR, after major refactoring or dependency upgrades, or pre-deploy.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
