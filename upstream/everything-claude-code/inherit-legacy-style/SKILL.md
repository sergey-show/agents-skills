---
id: everything-claude-code__inherit-legacy-style
name: inherit-legacy-style
version: 1.0.0
description: >-
  Prevent AI style drift on legacy projects by scanning the codebase for implicit conventions, resolving conflicts with the operator one at a time, and writing an enforceable .ai-style-rules.md (Golden Files, naming rules, DONTs) plus an optional CLAUDE.md hook. Use when onboarding an AI agent onto a hand-written legacy codebase or extracting a project's unwritten coding rules.
role: inherit-legacy-style
category: engineering
triggers:
  - inherit legacy style
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/inherit-legacy-style/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: inherit-legacy-style
---

# inherit-legacy-style

## Role

Portable distillation of upstream skill `inherit-legacy-style` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Prevent AI style drift on legacy projects by scanning the codebase for implicit conventions, resolving conflicts with the operator one at a time, and writing an enforceable .ai-style-rules.md (Golden Files, naming rules, DONTs) plus an optional CLAUDE.md hook. Use when onboarding an AI agent onto a hand-written legacy codebase or extracting a project's unwritten coding rules.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
