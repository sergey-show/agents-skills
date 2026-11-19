---
id: tokeneconomizer__config
name: config
version: 1.0.0
description: >-
  Show or change TokenEconomizer's settings: turn micro-skills, tool pruning or the loop guard on or off, or tune them, for this repository or (with --global) every repository. Use when the user asks to configure, enable or disable TokenEconomizer or one of its mechanisms.
role: config
category: meta
triggers:
  - config
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - shell.exec
sources:
  - research/TokenEconomizer/plugin/codex-skills/config/SKILL.md
harness: any
upstream_repo: TokenEconomizer
upstream_skill: config
---

# config

## Role

Portable distillation of upstream skill `config` from `TokenEconomizer`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Show or change TokenEconomizer's settings: turn micro-skills, tool pruning or the loop guard on or off, or tune them, for this repository or (with --global) every repository. Use when the user asks to configure, enable or disable TokenEconomizer or one of its mechanisms.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
