---
id: everything-claude-code__devfleet
name: devfleet
version: 1.0.0
description: >-
  Orchestrate multi-agent coding tasks via Claude DevFleet — plan projects, dispatch parallel agents in isolated worktrees, monitor progress, and read structured reports. Use when dispatching parallel coding agents across isolated worktrees and tracking their reports.
role: devfleet
category: meta
triggers:
  - devfleet
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/devfleet/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: devfleet
---

# devfleet

## Role

Portable distillation of upstream skill `devfleet` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Orchestrate multi-agent coding tasks via Claude DevFleet — plan projects, dispatch parallel agents in isolated worktrees, monitor progress, and read structured reports. Use when dispatching parallel coding agents across isolated worktrees and tracking their reports.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
