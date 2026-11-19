---
id: everything-claude-code__react-patterns
name: react-patterns
version: 1.0.0
description: >-
  React 18/19 patterns including hooks discipline, server/client component boundaries, Suspense + error boundaries, form actions, data fetching, state management decision trees, and accessibility-first composition. Use when writing or reviewing React components.
role: react-patterns
category: design
triggers:
  - react patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/react-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: react-patterns
---

# react-patterns

## Role

Portable distillation of upstream skill `react-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

React 18/19 patterns including hooks discipline, server/client component boundaries, Suspense + error boundaries, form actions, data fetching, state management decision trees, and accessibility-first composition. Use when writing or reviewing React components.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
