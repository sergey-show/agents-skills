---
id: everything-claude-code__conventional-commit-review
name: conventional-commit-review
version: 1.0.0
description: >-
  Reviews staged changes and drafts a Conventional Commits-compliant commit message with the right type, scope, and length. Use before committing, or when the user asks to write, fix, or review a commit message.
role: conventional-commit-review
category: engineering
triggers:
  - conventional commit review
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/conventional-commit-review/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: conventional-commit-review
---

# conventional-commit-review

## Role

Portable distillation of upstream skill `conventional-commit-review` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Reviews staged changes and drafts a Conventional Commits-compliant commit message with the right type, scope, and length. Use before committing, or when the user asks to write, fix, or review a commit message.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
