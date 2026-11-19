---
id: tokeneconomizer__repos
name: repos
version: 1.0.0
description: >-
  List every repository TokenEconomizer keeps state for (how each was identified, its agents and sessions, the checkouts seen), or merge one repository's state into another. Use when the user asks which repositories TokenEconomizer tracks, why state looks split or missing, or asks to merge or migrate it.
role: repos
category: meta
triggers:
  - repos
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - shell.exec
sources:
  - research/TokenEconomizer/plugin/codex-skills/repos/SKILL.md
harness: any
upstream_repo: TokenEconomizer
upstream_skill: repos
---

# repos

## Role

Portable distillation of upstream skill `repos` from `TokenEconomizer`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

List every repository TokenEconomizer keeps state for (how each was identified, its agents and sessions, the checkouts seen), or merge one repository's state into another. Use when the user asks which repositories TokenEconomizer tracks, why state looks split or missing, or asks to merge or migrate it.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
