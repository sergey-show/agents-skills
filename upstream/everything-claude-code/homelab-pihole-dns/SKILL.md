---
id: everything-claude-code__homelab-pihole-dns
name: homelab-pihole-dns
version: 1.0.0
description: >-
  Pi-hole installation, blocklist management, DNS-over-HTTPS setup, DHCP integration, local DNS records, and troubleshooting broken DNS resolution on a home network. Use when the task explicitly involves Pi-hole — installing it, managing blocklists, configuring DoH or DHCP, adding local DNS records, or diagnosing DNS resolution with Pi-hole in the path.
role: homelab-pihole-dns
category: engineering
triggers:
  - homelab pihole dns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/homelab-pihole-dns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: homelab-pihole-dns
---

# homelab-pihole-dns

## Role

Portable distillation of upstream skill `homelab-pihole-dns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Pi-hole installation, blocklist management, DNS-over-HTTPS setup, DHCP integration, local DNS records, and troubleshooting broken DNS resolution on a home network. Use when the task explicitly involves Pi-hole — installing it, managing blocklists, configuring DoH or DHCP, adding local DNS records, or diagnosing DNS resolution with Pi-hole in the path.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
