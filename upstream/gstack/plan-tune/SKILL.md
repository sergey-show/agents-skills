---
id: gstack__plan-tune
name: plan-tune
version: 1.0.0
description: >-
  Self-tuning question sensitivity + developer psychographic for gstack (v1: observational). Use for: tune questions, stop asking me that. (gstack)
role: plan-tune
category: meta
triggers:
  - plan tune
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/plan-tune/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: plan-tune
---

# plan-tune

## Role

Portable distillation of upstream skill `plan-tune` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Self-tuning question sensitivity + developer psychographic for gstack (v1: observational). Use for: tune questions, stop asking me that. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
