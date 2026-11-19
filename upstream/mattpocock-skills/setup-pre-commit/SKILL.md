---
id: mattpocock-skills__setup-pre-commit
name: setup-pre-commit
version: 1.0.0
description: >-
  Set up Husky pre-commit hooks with lint-staged (Prettier), type checking, and tests in the current repo. Use when user wants to add pre-commit hooks, set up Husky, configure lint-staged, or add commit-time formatting/typechecking/testing.
role: setup-pre-commit
category: engineering
triggers:
  - setup pre commit
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/skills/skills/misc/setup-pre-commit/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: setup-pre-commit
---

# setup-pre-commit

## Role

Portable distillation of upstream skill `setup-pre-commit` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Set up Husky pre-commit hooks with lint-staged (Prettier), type checking, and tests in the current repo. Use when user wants to add pre-commit hooks, set up Husky, configure lint-staged, or add commit-time formatting/typechecking/testing.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
