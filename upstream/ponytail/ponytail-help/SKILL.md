---
id: ponytail__ponytail-help
name: ponytail-help
version: 1.0.0
description: >-
  Quick reference for ponytail levels, skills and commands. One-shot display. Use for /ponytail-help, "ponytail help", "how do I use ponytail".
role: ponytail-help
category: engineering
triggers:
  - ponytail help
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - search.web
  - shell.exec
  - test.run
sources:
  - research/ponytail/skills/ponytail-help/SKILL.md
harness: any
upstream_repo: ponytail
upstream_skill: ponytail-help
---

# ponytail-help

## Role

Portable distillation of upstream skill `ponytail-help` from `ponytail`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Quick reference for ponytail levels, skills and commands. One-shot display. Use for /ponytail-help, "ponytail help", "how do I use ponytail".

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
