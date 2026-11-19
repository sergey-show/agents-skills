---
id: tokeneconomizer__microskills
name: microskills
version: 1.0.0
description: >-
  Show the repository facts (micro-skills) TokenEconomizer learned and injects at the start of each session here, and the ones still forming. Use when the user asks what TokenEconomizer learned or injects, or about its facts or micro-skills.
role: microskills
category: meta
triggers:
  - microskills
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - shell.exec
sources:
  - research/TokenEconomizer/plugin/codex-skills/microskills/SKILL.md
harness: any
upstream_repo: TokenEconomizer
upstream_skill: microskills
---

# microskills

## Role

Portable distillation of upstream skill `microskills` from `TokenEconomizer`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Show the repository facts (micro-skills) TokenEconomizer learned and injects at the start of each session here, and the ones still forming. Use when the user asks what TokenEconomizer learned or injects, or about its facts or micro-skills.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
