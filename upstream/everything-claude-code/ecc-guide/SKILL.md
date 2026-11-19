---
id: everything-claude-code__ecc-guide
name: ecc-guide
version: 1.0.0
description: >-
  Answer questions about ECC by reading the live repo surface — agents, skills, commands, hooks, rules, install profiles, and docs — instead of memory. Use when the user asks what ECC includes, how to install or reset it, which skill or command fits a task, or how project onboarding works.
role: ecc-guide
category: meta
triggers:
  - ecc guide
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/ecc-guide/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ecc-guide
---

# ecc-guide

## Role

Portable distillation of upstream skill `ecc-guide` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Answer questions about ECC by reading the live repo surface — agents, skills, commands, hooks, rules, install profiles, and docs — instead of memory. Use when the user asks what ECC includes, how to install or reset it, which skill or command fits a task, or how project onboarding works.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
