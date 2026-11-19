---
id: everything-claude-code__e2e-testing
name: e2e-testing
version: 1.0.0
description: >-
  Playwright E2E testing patterns, Page Object Model, configuration, CI/CD integration, artifact management, and flaky test strategies. Use when writing Playwright tests, structuring page objects, or fixing flaky E2E runs in CI.
role: e2e-testing
category: engineering
triggers:
  - e2e testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/e2e-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: e2e-testing
---

# e2e-testing

## Role

Portable distillation of upstream skill `e2e-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Playwright E2E testing patterns, Page Object Model, configuration, CI/CD integration, artifact management, and flaky test strategies. Use when writing Playwright tests, structuring page objects, or fixing flaky E2E runs in CI.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
