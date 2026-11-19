---
id: everything-claude-code__swiftui-patterns
name: swiftui-patterns
version: 1.0.0
description: >-
  SwiftUI architecture patterns, state management with @Observable, view composition, navigation, performance optimization, and modern iOS/macOS UI best practices. Use when building or reviewing SwiftUI views, @Observable state, navigation, or render performance.
role: swiftui-patterns
category: design
triggers:
  - swiftui patterns
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - test.run
sources:
  - research/everything-claude-code/skills/swiftui-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: swiftui-patterns
---

# swiftui-patterns

## Role

Portable distillation of upstream skill `swiftui-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

SwiftUI architecture patterns, state management with @Observable, view composition, navigation, performance optimization, and modern iOS/macOS UI best practices. Use when building or reviewing SwiftUI views, @Observable state, navigation, or render performance.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
