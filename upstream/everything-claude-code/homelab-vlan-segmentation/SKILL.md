---
id: everything-claude-code__homelab-vlan-segmentation
name: homelab-vlan-segmentation
version: 1.0.0
description: >-
  Segmenting home networks into VLANs for IoT, guest, trusted, and server traffic using UniFi, pfSense/OPNsense, and MikroTik — including switch trunk config, firewall rules, and wireless SSID mapping. Use when splitting a home network into IoT, guest, trusted, and server VLANs on UniFi, pfSense/OPNsense, or MikroTik.
role: homelab-vlan-segmentation
category: security
triggers:
  - homelab vlan segmentation
capabilities_required:
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/homelab-vlan-segmentation/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: homelab-vlan-segmentation
---

# homelab-vlan-segmentation

## Role

Portable distillation of upstream skill `homelab-vlan-segmentation` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Segmenting home networks into VLANs for IoT, guest, trusted, and server traffic using UniFi, pfSense/OPNsense, and MikroTik — including switch trunk config, firewall rules, and wireless SSID mapping. Use when splitting a home network into IoT, guest, trusted, and server VLANs on UniFi, pfSense/OPNsense, or MikroTik.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
