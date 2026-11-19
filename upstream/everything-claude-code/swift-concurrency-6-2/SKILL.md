---
id: everything-claude-code__swift-concurrency-6-2
name: swift-concurrency-6-2
version: 1.0.0
description: >-
  Swift 6.2 Approachable Concurrency — single-threaded by default, @concurrent for explicit background offloading, isolated conformances for main actor types. Use when adopting Swift 6.2 concurrency — offloading with @concurrent or resolving main-actor isolation.
role: swift-concurrency-6-2
category: design
triggers:
  - swift concurrency 6 2
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/swift-concurrency-6-2/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: swift-concurrency-6-2
---

# swift-concurrency-6-2

## Role

Portable distillation of upstream skill `swift-concurrency-6-2` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Swift 6.2 Approachable Concurrency — single-threaded by default, @concurrent for explicit background offloading, isolated conformances for main actor types. Use when adopting Swift 6.2 concurrency — offloading with @concurrent or resolving main-actor isolation.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
