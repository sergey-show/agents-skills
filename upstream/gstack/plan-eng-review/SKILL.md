---
id: gstack__plan-eng-review
name: plan-eng-review
version: 1.0.0
description: >-
  Use when you plan a feature before building it, or review a plan: locks in architecture, data flow, diagrams, edge cases, test coverage and performance. Use for: plan a feature, review architecture, eng plan review. (gstack)
role: plan-eng-review
category: meta
triggers:
  - plan eng review
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/plan-eng-review/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: plan-eng-review
---

# plan-eng-review

## Role

Portable distillation of upstream skill `plan-eng-review` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when you plan a feature before building it, or review a plan: locks in architecture, data flow, diagrams, edge cases, test coverage and performance. Use for: plan a feature, review architecture, eng plan review. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
