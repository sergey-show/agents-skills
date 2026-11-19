---
id: everything-claude-code__homelab-wireguard-vpn
name: homelab-wireguard-vpn
version: 1.0.0
description: >-
  WireGuard VPN server setup, peer configuration, key generation, split tunneling vs full tunnel routing, and remote access to a home network from mobile and laptop clients. Use when setting up WireGuard for remote access to a home network, or deciding between split and full tunnel routing.
role: homelab-wireguard-vpn
category: engineering
triggers:
  - homelab wireguard vpn
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/homelab-wireguard-vpn/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: homelab-wireguard-vpn
---

# homelab-wireguard-vpn

## Role

Portable distillation of upstream skill `homelab-wireguard-vpn` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

WireGuard VPN server setup, peer configuration, key generation, split tunneling vs full tunnel routing, and remote access to a home network from mobile and laptop clients. Use when setting up WireGuard for remote access to a home network, or deciding between split and full tunnel routing.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
