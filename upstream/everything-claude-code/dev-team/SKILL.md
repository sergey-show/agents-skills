---
id: everything-claude-code__dev-team
name: dev-team
version: 1.0.0
description: >-
  Simulate a collaborative dev team session where multiple role-based personas (PM, Architect, Developer, QA) respond to the same problem together in one session. Use when designing a feature, reviewing a proposal, or onboarding a new initiative and you want multi-role perspective without switching agents manually.
role: dev-team
category: design
triggers:
  - dev team
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
  - research/everything-claude-code/skills/dev-team/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: dev-team
---

# dev-team

## Role

Portable distillation of upstream skill `dev-team` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Simulate a collaborative dev team session where multiple role-based personas (PM, Architect, Developer, QA) respond to the same problem together in one session. Use when designing a feature, reviewing a proposal, or onboarding a new initiative and you want multi-role perspective without switching agents manually.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
