---
id: everything-claude-code__operator-approval-loop
name: operator-approval-loop
version: 1.0.0
description: >-
  Operator approval contract with internal filing notices for agent-drafted outbound messages, hashed drafts, epoch-keyed decisions, durable delivery claims and receipts, and a pre-draft baseline gate. Use when an agent drafts messages to external counterparties and a human operator must approve, reject, or steer each send before it leaves.
role: operator-approval-loop
category: meta
triggers:
  - operator approval loop
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
  - research/everything-claude-code/skills/operator-approval-loop/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: operator-approval-loop
---

# operator-approval-loop

## Role

Portable distillation of upstream skill `operator-approval-loop` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Operator approval contract with internal filing notices for agent-drafted outbound messages, hashed drafts, epoch-keyed decisions, durable delivery claims and receipts, and a pre-draft baseline gate. Use when an agent drafts messages to external counterparties and a human operator must approve, reject, or steer each send before it leaves.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
