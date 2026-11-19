---
id: rea__rea-ci-tests-audit
name: rea-ci-tests-audit
version: 1.0.0
description: >-
  Audit REA CI and test suites for correctness, fixture drift, false passes, and measured performance; use for suite or workflow investigations and efficiency changes, rather than ordinary feature testing or a single test failure.
role: rea-ci-tests-audit
category: engineering
triggers:
  - rea ci tests audit
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/rea/.agents/skills/rea-ci-tests-audit/SKILL.md
harness: any
upstream_repo: rea
upstream_skill: rea-ci-tests-audit
---

# rea-ci-tests-audit

## Role

Portable distillation of upstream skill `rea-ci-tests-audit` from `rea`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Audit REA CI and test suites for correctness, fixture drift, false passes, and measured performance; use for suite or workflow investigations and efficiency changes, rather than ordinary feature testing or a single test failure.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
