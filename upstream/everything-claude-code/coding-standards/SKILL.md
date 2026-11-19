---
id: everything-claude-code__coding-standards
name: coding-standards
version: 1.0.0
description: >-
  Baseline cross-project coding conventions for naming, readability, immutability, and code-quality review. Use detailed frontend or backend skills for framework-specific patterns. Use when reviewing code quality or naming with no framework-specific skill that applies.
role: coding-standards
category: design
triggers:
  - coding standards
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/coding-standards/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: coding-standards
---

# coding-standards

## Role

Portable distillation of upstream skill `coding-standards` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Baseline cross-project coding conventions for naming, readability, immutability, and code-quality review. Use detailed frontend or backend skills for framework-specific patterns. Use when reviewing code quality or naming with no framework-specific skill that applies.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
