---
id: gstack__autoplan
name: autoplan
version: 1.0.0
description: >-
  Auto-review pipeline — runs the CEO, design, eng and DX reviews in order (lean run: one reviewer), auto-deciding. Use for: run all reviews, automatic review pipeline. (gstack)
role: autoplan
category: meta
triggers:
  - autoplan
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/autoplan/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: autoplan
---

# autoplan

## Role

Portable distillation of upstream skill `autoplan` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Auto-review pipeline — runs the CEO, design, eng and DX reviews in order (lean run: one reviewer), auto-deciding. Use for: run all reviews, automatic review pipeline. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
