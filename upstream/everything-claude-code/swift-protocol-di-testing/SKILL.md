---
id: everything-claude-code__swift-protocol-di-testing
name: swift-protocol-di-testing
version: 1.0.0
description: >-
  Protocol-based dependency injection for testable Swift code — mock file system, network, and external APIs using focused protocols and Swift Testing. Use when Swift code needs testing and file system, network, or external APIs must be mocked.
role: swift-protocol-di-testing
category: design
triggers:
  - swift protocol di testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/swift-protocol-di-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: swift-protocol-di-testing
---

# swift-protocol-di-testing

## Role

Portable distillation of upstream skill `swift-protocol-di-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Protocol-based dependency injection for testable Swift code — mock file system, network, and external APIs using focused protocols and Swift Testing. Use when Swift code needs testing and file system, network, or external APIs must be mocked.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
