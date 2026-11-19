---
id: everything-claude-code__connections-optimizer
name: connections-optimizer
version: 1.0.0
description: >-
  Reorganize the user's X and LinkedIn network with review-first pruning, add/follow recommendations, and channel-specific warm outreach drafted in the user's real voice. Use when the user wants to clean up following lists, grow toward current priorities, or rebalance a social graph around higher-signal relationships.
role: connections-optimizer
category: meta
triggers:
  - connections optimizer
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
sources:
  - research/everything-claude-code/skills/connections-optimizer/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: connections-optimizer
---

# connections-optimizer

## Role

Portable distillation of upstream skill `connections-optimizer` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Reorganize the user's X and LinkedIn network with review-first pruning, add/follow recommendations, and channel-specific warm outreach drafted in the user's real voice. Use when the user wants to clean up following lists, grow toward current priorities, or rebalance a social graph around higher-signal relationships.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
