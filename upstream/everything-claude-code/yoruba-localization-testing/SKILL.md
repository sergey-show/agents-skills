---
id: everything-claude-code__yoruba-localization-testing
name: yoruba-localization-testing
version: 1.0.0
description: >-
  Test Yoruba (yo) and English bilingual interfaces for tone marks, underdots, Unicode normalization, translation fallback, and accessibility.
role: yoruba-localization-testing
category: meta
triggers:
  - yoruba localization testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - test.run
sources:
  - research/everything-claude-code/skills/yoruba-localization-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: yoruba-localization-testing
---

# yoruba-localization-testing

## Role

Portable distillation of upstream skill `yoruba-localization-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Test Yoruba (yo) and English bilingual interfaces for tone marks, underdots, Unicode normalization, translation fallback, and accessibility.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
