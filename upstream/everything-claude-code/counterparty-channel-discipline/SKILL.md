---
id: everything-claude-code__counterparty-channel-discipline
name: counterparty-channel-discipline
version: 1.0.0
description: >-
  Per-channel strict prompts, mention gating, silent observation, and a communication autonomy policy for agents that sit in shared channels with external counterparties. Use when an agent joins group chats, shared channels, or DMs where outsiders can read every message and you need it to speak only when addressed, never leak internal context, and route risky content to draft-only approval.
role: counterparty-channel-discipline
category: meta
triggers:
  - counterparty channel discipline
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
  - research/everything-claude-code/skills/counterparty-channel-discipline/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: counterparty-channel-discipline
---

# counterparty-channel-discipline

## Role

Portable distillation of upstream skill `counterparty-channel-discipline` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Per-channel strict prompts, mention gating, silent observation, and a communication autonomy policy for agents that sit in shared channels with external counterparties. Use when an agent joins group chats, shared channels, or DMs where outsiders can read every message and you need it to speak only when addressed, never leak internal context, and route risky content to draft-only approval.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
