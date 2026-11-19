---
id: everything-claude-code__network-bgp-diagnostics
name: network-bgp-diagnostics
version: 1.0.0
description: >-
  Diagnostics-only BGP troubleshooting patterns for neighbor state, route exchange, prefix policy, AS path inspection, and safe evidence collection. Use when a BGP neighbor is down, routes are missing, or prefix policy and AS path need inspection.
role: network-bgp-diagnostics
category: meta
triggers:
  - network bgp diagnostics
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/network-bgp-diagnostics/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: network-bgp-diagnostics
---

# network-bgp-diagnostics

## Role

Portable distillation of upstream skill `network-bgp-diagnostics` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Diagnostics-only BGP troubleshooting patterns for neighbor state, route exchange, prefix policy, AS path inspection, and safe evidence collection. Use when a BGP neighbor is down, routes are missing, or prefix policy and AS path need inspection.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
