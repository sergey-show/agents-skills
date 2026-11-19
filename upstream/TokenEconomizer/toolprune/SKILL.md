---
id: tokeneconomizer__toolprune
name: toolprune
version: 1.0.0
description: >-
  Review, undo or apply TokenEconomizer's deny list of Codex capabilities this repository never uses (written to the project's .codex/config.toml). Use when the user asks about TokenEconomizer's tool pruning or deny list, or asks to restore or apply it.
role: toolprune
category: meta
triggers:
  - toolprune
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - shell.exec
sources:
  - research/TokenEconomizer/plugin/codex-skills/toolprune/SKILL.md
harness: any
upstream_repo: TokenEconomizer
upstream_skill: toolprune
---

# toolprune

## Role

Portable distillation of upstream skill `toolprune` from `TokenEconomizer`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Review, undo or apply TokenEconomizer's deny list of Codex capabilities this repository never uses (written to the project's .codex/config.toml). Use when the user asks about TokenEconomizer's tool pruning or deny list, or asks to restore or apply it.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
