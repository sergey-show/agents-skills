---
id: everything-claude-code__dynamic-workflow-mode
name: dynamic-workflow-mode
version: 1.0.0
description: >-
  Design task-local harnesses, eval gates, and reusable skill extraction for Claude dynamic workflow mode and other adaptive agent harnesses. Use when building a task-local harness, adding eval gates, or extracting a reusable skill from ad-hoc work.
role: dynamic-workflow-mode
category: meta
triggers:
  - dynamic workflow mode
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/dynamic-workflow-mode/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: dynamic-workflow-mode
---

# dynamic-workflow-mode

## Role

Portable distillation of upstream skill `dynamic-workflow-mode` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design task-local harnesses, eval gates, and reusable skill extraction for Claude dynamic workflow mode and other adaptive agent harnesses. Use when building a task-local harness, adding eval gates, or extracting a reusable skill from ad-hoc work.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
