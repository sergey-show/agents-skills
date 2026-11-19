---
id: everything-claude-code__plan-canvas
name: plan-canvas
version: 1.0.0
description: >-
  Open plans and HTML artifacts in a local browser canvas where the human annotates elements, chats, and approves or requests changes without leaving the page. Use when presenting a plan for review, or when feedback like "move this, change that" is easier pointed at than typed.
role: plan-canvas
category: engineering
triggers:
  - plan canvas
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/plan-canvas/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: plan-canvas
---

# plan-canvas

## Role

Portable distillation of upstream skill `plan-canvas` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Open plans and HTML artifacts in a local browser canvas where the human annotates elements, chats, and approves or requests changes without leaving the page. Use when presenting a plan for review, or when feedback like "move this, change that" is easier pointed at than typed.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
