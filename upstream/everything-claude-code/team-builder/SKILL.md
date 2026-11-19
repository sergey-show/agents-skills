---
id: everything-claude-code__team-builder
name: team-builder
version: 1.0.0
description: >-
  Interactive picker that discovers available agent personas via the claude agents command and agents/ markdown globs, groups them into domains, has the user select up to five, dispatches them in parallel on one task, and synthesizes agreements and conflicts into a unified report. Use when composing a team of agents, browsing available agent personas, or running several specialist agents in parallel.
role: team-builder
category: security
triggers:
  - team builder
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/team-builder/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: team-builder
---

# team-builder

## Role

Portable distillation of upstream skill `team-builder` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Interactive picker that discovers available agent personas via the claude agents command and agents/ markdown globs, groups them into domains, has the user select up to five, dispatches them in parallel on one task, and synthesizes agreements and conflicts into a unified report. Use when composing a team of agents, browsing available agent personas, or running several specialist agents in parallel.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
