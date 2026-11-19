---
id: agent-skills__shipping-and-launch
name: shipping-and-launch
version: 1.0.0
description: >-
  Prepares production launches. Use when preparing to deploy to production, or when asking what needs to be in place before shipping. Use when you need a pre-launch checklist, when setting up monitoring, when planning a staged rollout, or when you need a rollback strategy.
role: shipping-and-launch
category: ops
triggers:
  - shipping and launch
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/shipping-and-launch/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: shipping-and-launch
---

# shipping-and-launch

## Role

Portable distillation of upstream skill `shipping-and-launch` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Prepares production launches. Use when preparing to deploy to production, or when asking what needs to be in place before shipping. Use when you need a pre-launch checklist, when setting up monitoring, when planning a staged rollout, or when you need a rollback strategy.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
