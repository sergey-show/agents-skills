---
id: everything-claude-code__crosspost
name: crosspost
version: 1.0.0
description: >-
  Multi-platform content distribution across X, LinkedIn, Threads, and Bluesky. Adapts content per platform using content-engine patterns. Never posts identical content cross-platform. Use when the user wants to distribute content across social platforms.
role: crosspost
category: ops
triggers:
  - crosspost
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/.agents/skills/crosspost/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: crosspost
---

# crosspost

## Role

Portable distillation of upstream skill `crosspost` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Multi-platform content distribution across X, LinkedIn, Threads, and Bluesky. Adapts content per platform using content-engine patterns. Never posts identical content cross-platform. Use when the user wants to distribute content across social platforms.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
