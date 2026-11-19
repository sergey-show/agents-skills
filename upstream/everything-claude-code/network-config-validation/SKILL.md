---
id: everything-claude-code__network-config-validation
name: network-config-validation
version: 1.0.0
description: >-
  Pre-deployment checks for router and switch configuration, including dangerous commands, duplicate addresses, subnet overlaps, stale references, management-plane risk, and IOS-style security hygiene. Use when reviewing a router or switch configuration before deployment.
role: network-config-validation
category: ops
triggers:
  - network config validation
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/network-config-validation/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: network-config-validation
---

# network-config-validation

## Role

Portable distillation of upstream skill `network-config-validation` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Pre-deployment checks for router and switch configuration, including dangerous commands, duplicate addresses, subnet overlaps, stale references, management-plane risk, and IOS-style security hygiene. Use when reviewing a router or switch configuration before deployment.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
