---
id: everything-claude-code__netmiko-ssh-automation
name: netmiko-ssh-automation
version: 1.0.0
description: >-
  Safe Python Netmiko patterns for read-only collection, bounded batch SSH, TextFSM parsing, guarded config changes, timeouts, and network automation error handling. Use when automating network device access with Python Netmiko, whether collecting state or pushing guarded config changes.
role: netmiko-ssh-automation
category: meta
triggers:
  - netmiko ssh automation
capabilities_required:
  - filesystem.read
capabilities_optional:
  - ask_user
  - shell.exec
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/netmiko-ssh-automation/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: netmiko-ssh-automation
---

# netmiko-ssh-automation

## Role

Portable distillation of upstream skill `netmiko-ssh-automation` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Safe Python Netmiko patterns for read-only collection, bounded batch SSH, TextFSM parsing, guarded config changes, timeouts, and network automation error handling. Use when automating network device access with Python Netmiko, whether collecting state or pushing guarded config changes.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
