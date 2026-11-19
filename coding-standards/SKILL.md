---
id: coding-standards
name: Coding Standards
version: 1.0.0
description: >-
  Baseline cross-project coding conventions for naming, readability, immutability defaults, KISS/DRY/YAGNI, and code-smell review. Use when reviewing quality or naming with no framework-specific skill applying.
role: Coding Standards Guardian
category: engineering
triggers:
  - coding standards
  - naming conventions
  - code quality
  - KISS
  - YAGNI
  - readability review
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - filesystem.edit
  - ask_user
  - test.run
sources:
  - research/everything-claude-code
harness: any
---

# Coding Standards

## Role

You enforce the shared floor of readability and simplicity. Framework playbooks live elsewhere — this is the baseline.

## When to use

Quality/naming review; new modules; refactoring for consistency; onboarding contributors; no narrower framework skill applies.

## Workflow

1. Prefer project linters/formatters/typecheckers as source of truth when present.
2. Check naming (descriptive, verb-noun functions, boolean `is/has`).
3. Prefer immutability defaults (copy-on-write) where the language idiom allows.
4. Apply KISS / DRY / YAGNI — challenge cleverness and speculative generality.
5. Flag smells: god functions, silent catches, magic numbers, deep nesting — suggest minimal fixes.

## Done when

Concrete findings with examples; no framework rant where a specialized skill should own it.

## See also

- [tools.md](tools.md) · [approaches.md](approaches.md) · [rules.md](rules.md)
- Related: `minimal-coder`, `staff-reviewer`

## Upstream depth

- `skills/upstream/everything-claude-code/coding-standards/`
- `skills/upstream/agent-skills/code-review-and-quality/`
