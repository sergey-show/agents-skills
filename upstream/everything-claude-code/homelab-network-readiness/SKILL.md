---
id: everything-claude-code__homelab-network-readiness
name: homelab-network-readiness
version: 1.0.0
description: >-
  Readiness checklist for homelab VLAN segmentation, local DNS filtering (Pi-hole, AdGuard Home), and WireGuard-style remote access. Use when planning or reviewing home network changes — splitting a flat network into trusted, IoT, guest, or management VLANs, moving DHCP to a local resolver, or adding VPN access — before changing router, firewall, DHCP, or VPN configuration.
role: homelab-network-readiness
category: meta
triggers:
  - homelab network readiness
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/homelab-network-readiness/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: homelab-network-readiness
---

# homelab-network-readiness

## Role

Portable distillation of upstream skill `homelab-network-readiness` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Readiness checklist for homelab VLAN segmentation, local DNS filtering (Pi-hole, AdGuard Home), and WireGuard-style remote access. Use when planning or reviewing home network changes — splitting a flat network into trusted, IoT, guest, or management VLANs, moving DHCP to a local resolver, or adding VPN access — before changing router, firewall, DHCP, or VPN configuration.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
