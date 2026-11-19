---
id: everything-claude-code__team-agent-orchestration
name: team-agent-orchestration
version: 1.0.0
description: >-
  Run team-based orchestration for agent squads: work items with owners and scope, agent Kanban state, branch isolation, control pane visibility, and merge gates. Use when coordinating multiple agents in parallel across branches or worktrees — multi-agent fan-out, agent Kanban, squad coordination, or merging agent output into one product.
role: team-agent-orchestration
category: ops
triggers:
  - team agent orchestration
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/team-agent-orchestration/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: team-agent-orchestration
---

# team-agent-orchestration

## Role

Portable distillation of upstream skill `team-agent-orchestration` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Run team-based orchestration for agent squads: work items with owners and scope, agent Kanban state, branch isolation, control pane visibility, and merge gates. Use when coordinating multiple agents in parallel across branches or worktrees — multi-agent fan-out, agent Kanban, squad coordination, or merging agent output into one product.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
