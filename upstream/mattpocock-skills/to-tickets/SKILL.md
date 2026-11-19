---
id: mattpocock-skills__to-tickets
name: to-tickets
version: 1.0.0
description: >-
  Break a plan, spec, or the current conversation into a set of tracer-bullet tickets, each declaring its blocking edges, published to the configured tracker (edges as text in one file per ticket locally, or native blocking links on a real tracker).
role: to-tickets
category: meta
triggers:
  - to tickets
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/skills/skills/engineering/to-tickets/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: to-tickets
---

# to-tickets

## Role

Portable distillation of upstream skill `to-tickets` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Break a plan, spec, or the current conversation into a set of tracer-bullet tickets, each declaring its blocking edges, published to the configured tracker (edges as text in one file per ticket locally, or native blocking links on a real tracker).

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
