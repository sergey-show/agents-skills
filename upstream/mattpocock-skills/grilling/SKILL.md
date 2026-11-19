---
id: mattpocock-skills__grilling
name: grilling
version: 1.0.0
description: >-
  Grill the user relentlessly about a plan, decision, or idea. Use when the user wants to stress-test their thinking, or uses any 'grill' trigger phrases.
role: grilling
category: design
triggers:
  - grilling
capabilities_required:
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - subagent.spawn
sources:
  - research/skills/skills/productivity/grilling/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: grilling
---

# grilling

## Role

Portable distillation of upstream skill `grilling` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Grill the user relentlessly about a plan, decision, or idea. Use when the user wants to stress-test their thinking, or uses any 'grill' trigger phrases.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
