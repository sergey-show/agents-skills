---
id: everything-claude-code__context-budget
name: context-budget
version: 1.0.0
description: >-
  Routes live context checks to the native Codex or the coding agent meter without scanning files, and performs a bounded static component audit only when explicitly requested. Use for context-budget requests about remaining capacity or installed context overhead.
role: context-budget
category: meta
triggers:
  - context budget
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/context-budget/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: context-budget
---

# context-budget

## Role

Portable distillation of upstream skill `context-budget` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Routes live context checks to the native Codex or the coding agent meter without scanning files, and performs a bounded static component audit only when explicitly requested. Use for context-budget requests about remaining capacity or installed context overhead.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
