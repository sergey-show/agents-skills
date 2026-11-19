---
id: everything-claude-code__perl-testing
name: perl-testing
version: 1.0.0
description: >-
  Perl testing patterns using Test2::V0, Test::More, prove runner, mocking, coverage with Devel::Cover, and TDD methodology. Use when writing Perl tests with Test2::V0 or Test::More, or measuring coverage.
role: perl-testing
category: design
triggers:
  - perl testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/perl-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: perl-testing
---

# perl-testing

## Role

Portable distillation of upstream skill `perl-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Perl testing patterns using Test2::V0, Test::More, prove runner, mocking, coverage with Devel::Cover, and TDD methodology. Use when writing Perl tests with Test2::V0 or Test::More, or measuring coverage.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
