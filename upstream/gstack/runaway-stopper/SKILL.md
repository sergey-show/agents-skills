---
id: gstack__runaway-stopper
name: runaway-stopper
version: 1.0.0
description: >-
  Find runaway Capy threads and subagents, stop or rotate them safely, and prevent repeats. Use for: find runaway threads, stop runaway jobs. (gstack)
role: runaway-stopper
category: meta
triggers:
  - runaway stopper
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/runaway-stopper/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: runaway-stopper
---

# runaway-stopper

## Role

Portable distillation of upstream skill `runaway-stopper` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Find runaway Capy threads and subagents, stop or rotate them safely, and prevent repeats. Use for: find runaway threads, stop runaway jobs. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
