---
id: everything-claude-code__i18n-sync
name: i18n-sync
version: 1.0.0
description: >-
  Translate and synchronize application JSON locale files using source-key usage, project terminology, and focused validation. Use when adding keys or languages, updating source copy, or reviewing missing and stale translations.
role: i18n-sync
category: engineering
triggers:
  - i18n sync
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/i18n-sync/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: i18n-sync
---

# i18n-sync

## Role

Portable distillation of upstream skill `i18n-sync` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Translate and synchronize application JSON locale files using source-key usage, project terminology, and focused validation. Use when adding keys or languages, updating source copy, or reviewing missing and stale translations.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
