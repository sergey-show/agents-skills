---
id: everything-claude-code__compose-multiplatform-patterns
name: compose-multiplatform-patterns
version: 1.0.0
description: >-
  Compose Multiplatform and Jetpack Compose patterns for KMP projects — state management, navigation, theming, performance, and platform-specific UI. Use when building Compose or Jetpack Compose UI, state, navigation, or theming in a KMP project.
role: compose-multiplatform-patterns
category: design
triggers:
  - compose multiplatform patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - test.run
sources:
  - research/everything-claude-code/skills/compose-multiplatform-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: compose-multiplatform-patterns
---

# compose-multiplatform-patterns

## Role

Portable distillation of upstream skill `compose-multiplatform-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Compose Multiplatform and Jetpack Compose patterns for KMP projects — state management, navigation, theming, performance, and platform-specific UI. Use when building Compose or Jetpack Compose UI, state, navigation, or theming in a KMP project.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
