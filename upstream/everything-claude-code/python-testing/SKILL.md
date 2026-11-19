---
id: everything-claude-code__python-testing
name: python-testing
version: 1.0.0
description: >-
  Python testing strategies using pytest, TDD methodology, fixtures, mocking, parametrization, and coverage requirements. Use when writing pytest tests — fixtures, mocks, parametrization, or coverage.
role: python-testing
category: design
triggers:
  - python testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/python-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: python-testing
---

# python-testing

## Role

Portable distillation of upstream skill `python-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Python testing strategies using pytest, TDD methodology, fixtures, mocking, parametrization, and coverage requirements. Use when writing pytest tests — fixtures, mocks, parametrization, or coverage.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
