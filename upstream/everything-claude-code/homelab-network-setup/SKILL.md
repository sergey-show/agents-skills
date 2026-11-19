---
id: everything-claude-code__homelab-network-setup
name: homelab-network-setup
version: 1.0.0
description: >-
  Practical home and homelab network planning for gateways, switches, access points, IP ranges, DHCP reservations, DNS, cabling, and common beginner mistakes. Use when planning or fixing a home or homelab network — gateway, switch, AP, IP ranges, DHCP, DNS, or cabling.
role: homelab-network-setup
category: design
triggers:
  - homelab network setup
capabilities_required:
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/homelab-network-setup/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: homelab-network-setup
---

# homelab-network-setup

## Role

Portable distillation of upstream skill `homelab-network-setup` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Practical home and homelab network planning for gateways, switches, access points, IP ranges, DHCP reservations, DNS, cabling, and common beginner mistakes. Use when planning or fixing a home or homelab network — gateway, switch, AP, IP ranges, DHCP, DNS, or cabling.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
