---
id: gstack__captain
name: captain
version: 1.0.0
description: >-
  Run a crew of coding agents from one controller (also /crew): lanes send READY blocks and never merge; the controller merges through trains, keeps the digest, relays approvals, fixes flakes daily. Use for: captain, crew. (gstack)
role: captain
category: meta
triggers:
  - captain
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/captain/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: captain
---

# captain

## Role

Portable distillation of upstream skill `captain` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Run a crew of coding agents from one controller (also /crew): lanes send READY blocks and never merge; the controller merges through trains, keeps the digest, relays approvals, fixes flakes daily. Use for: captain, crew. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
