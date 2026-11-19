---
id: mattpocock-skills__tdd
name: tdd
version: 1.0.0
description: >-
  Test-driven development. Use when the user wants to build features or fix bugs test-first, mentions "red-green-refactor", or wants integration tests.
role: tdd
category: meta
triggers:
  - tdd
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/skills/skills/engineering/tdd/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: tdd
---

# tdd

## Role

Portable distillation of upstream skill `tdd` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Test-driven development. Use when the user wants to build features or fix bugs test-first, mentions "red-green-refactor", or wants integration tests.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
