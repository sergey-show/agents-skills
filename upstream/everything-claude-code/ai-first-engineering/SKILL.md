---
id: everything-claude-code__ai-first-engineering
name: ai-first-engineering
version: 1.0.0
description: >-
  Engineering operating model for teams where AI agents generate a large share of implementation output. Use when setting team process, review gates, or ownership rules for a codebase largely written by agents.
role: ai-first-engineering
category: design
triggers:
  - ai first engineering
capabilities_required:
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/ai-first-engineering/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ai-first-engineering
---

# ai-first-engineering

## Role

Portable distillation of upstream skill `ai-first-engineering` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Engineering operating model for teams where AI agents generate a large share of implementation output. Use when setting team process, review gates, or ownership rules for a codebase largely written by agents.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
