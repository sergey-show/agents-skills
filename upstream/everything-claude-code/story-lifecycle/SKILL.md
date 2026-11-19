---
id: everything-claude-code__story-lifecycle
name: story-lifecycle
version: 1.0.0
description: >-
  Manage a file-based epic → story → sprint development loop without requiring an external project management tool. Creates and tracks epics, breaks them into user stories, assigns them to sprints, and drives implementation story by story. Use when starting a new feature initiative or when the team has no Jira/Linear/Taiga but needs structured delivery tracking.
role: story-lifecycle
category: engineering
triggers:
  - story lifecycle
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/story-lifecycle/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: story-lifecycle
---

# story-lifecycle

## Role

Portable distillation of upstream skill `story-lifecycle` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Manage a file-based epic → story → sprint development loop without requiring an external project management tool. Creates and tracks epics, breaks them into user stories, assigns them to sprints, and drives implementation story by story. Use when starting a new feature initiative or when the team has no Jira/Linear/Taiga but needs structured delivery tracking.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
