---
id: everything-claude-code__cisco-ios-patterns
name: cisco-ios-patterns
version: 1.0.0
description: >-
  Cisco IOS and IOS-XE review patterns for show commands, config hierarchy, wildcard masks, ACL placement, interface hygiene, and safe change-window verification. Use when reading, writing, or reviewing Cisco IOS / IOS-XE configuration or planning a change window.
role: cisco-ios-patterns
category: meta
triggers:
  - cisco ios patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/cisco-ios-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: cisco-ios-patterns
---

# cisco-ios-patterns

## Role

Portable distillation of upstream skill `cisco-ios-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Cisco IOS and IOS-XE review patterns for show commands, config hierarchy, wildcard masks, ACL placement, interface hygiene, and safe change-window verification. Use when reading, writing, or reviewing Cisco IOS / IOS-XE configuration or planning a change window.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
