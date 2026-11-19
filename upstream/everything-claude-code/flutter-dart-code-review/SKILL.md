---
id: everything-claude-code__flutter-dart-code-review
name: flutter-dart-code-review
version: 1.0.0
description: >-
  Library-agnostic Flutter/Dart code review checklist covering widget best practices, state management patterns (BLoC, Riverpod, Provider, GetX, MobX, Signals), Dart idioms, performance, accessibility, security, and clean architecture. Use when reviewing Flutter or Dart code, whatever state management library the project uses.
role: flutter-dart-code-review
category: engineering
triggers:
  - flutter dart code review
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/flutter-dart-code-review/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: flutter-dart-code-review
---

# flutter-dart-code-review

## Role

Portable distillation of upstream skill `flutter-dart-code-review` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Library-agnostic Flutter/Dart code review checklist covering widget best practices, state management patterns (BLoC, Riverpod, Provider, GetX, MobX, Signals), Dart idioms, performance, accessibility, security, and clean architecture. Use when reviewing Flutter or Dart code, whatever state management library the project uses.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
