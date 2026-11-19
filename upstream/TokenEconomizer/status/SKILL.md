---
id: tokeneconomizer__status
name: status
version: 1.0.0
description: >-
  Show what TokenEconomizer has learned for this repository, what it has done, and what this repository's sessions cost. Use when the user asks about TokenEconomizer, its status, its savings or overhead, or what it learned here.
role: status
category: meta
triggers:
  - status
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - shell.exec
sources:
  - research/TokenEconomizer/plugin/codex-skills/status/SKILL.md
harness: any
upstream_repo: TokenEconomizer
upstream_skill: status
---

# status

## Role

Portable distillation of upstream skill `status` from `TokenEconomizer`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Show what TokenEconomizer has learned for this repository, what it has done, and what this repository's sessions cost. Use when the user asks about TokenEconomizer, its status, its savings or overhead, or what it learned here.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
