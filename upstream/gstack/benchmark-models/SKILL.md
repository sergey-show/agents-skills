---
id: gstack__benchmark-models
name: benchmark-models
version: 1.0.0
description: >-
  Cross-model benchmark for gstack skills. Use for: cross model benchmark, compare claude gpt gemini. (gstack)
role: benchmark-models
category: meta
triggers:
  - benchmark models
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/benchmark-models/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: benchmark-models
---

# benchmark-models

## Role

Portable distillation of upstream skill `benchmark-models` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Cross-model benchmark for gstack skills. Use for: cross model benchmark, compare claude gpt gemini. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
