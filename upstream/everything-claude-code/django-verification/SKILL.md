---
id: everything-claude-code__django-verification
name: django-verification
version: 1.0.0
description: >-
  Run the full Django verification loop — environment check, mypy/ruff/black linting, migration safety, pytest with coverage targets, pip-audit and bandit security scans, settings and logging review, and diff review — producing a phased pass/fail report before release or PR. Use when preparing a Django pull request, validating migrations or coverage, or running pre-deploy readiness checks.
role: django-verification
category: security
triggers:
  - django verification
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/django-verification/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: django-verification
---

# django-verification

## Role

Portable distillation of upstream skill `django-verification` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Run the full Django verification loop — environment check, mypy/ruff/black linting, migration safety, pytest with coverage targets, pip-audit and bandit security scans, settings and logging review, and diff review — producing a phased pass/fail report before release or PR. Use when preparing a Django pull request, validating migrations or coverage, or running pre-deploy readiness checks.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
