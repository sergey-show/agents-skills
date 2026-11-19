---
id: everything-claude-code__swift-actor-persistence
name: swift-actor-persistence
version: 1.0.0
description: >-
  Thread-safe data persistence in Swift using actors — in-memory cache with file-backed storage, eliminating data races by design. Use when persisting data in Swift and a data race or thread-safety problem needs designing out.
role: swift-actor-persistence
category: meta
triggers:
  - swift actor persistence
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/swift-actor-persistence/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: swift-actor-persistence
---

# swift-actor-persistence

## Role

Portable distillation of upstream skill `swift-actor-persistence` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Thread-safe data persistence in Swift using actors — in-memory cache with file-backed storage, eliminating data races by design. Use when persisting data in Swift and a data race or thread-safety problem needs designing out.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
