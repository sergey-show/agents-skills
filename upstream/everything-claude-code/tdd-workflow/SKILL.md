---
id: everything-claude-code__tdd-workflow
name: tdd-workflow
version: 1.0.0
description: >-
  Use this skill when writing new features, fixing bugs, or refactoring code. Enforces test-driven development with 80%+ coverage including unit, integration, and E2E tests.
role: tdd-workflow
category: meta
triggers:
  - tdd workflow
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
  - research/everything-claude-code/.agents/skills/tdd-workflow/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: tdd-workflow
---

# tdd-workflow

## Role

Portable distillation of upstream skill `tdd-workflow` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use this skill when writing new features, fixing bugs, or refactoring code. Enforces test-driven development with 80%+ coverage including unit, integration, and E2E tests.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
