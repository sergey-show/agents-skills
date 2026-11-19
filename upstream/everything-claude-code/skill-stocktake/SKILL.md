---
id: everything-claude-code__skill-stocktake
name: skill-stocktake
version: 1.0.0
description: >-
  Use when auditing Claude skills and commands for quality. Supports Quick Scan (changed skills only) and Full Stocktake modes with sequential subagent batch evaluation.
role: skill-stocktake
category: meta
triggers:
  - skill stocktake
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/skill-stocktake/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: skill-stocktake
---

# skill-stocktake

## Role

Portable distillation of upstream skill `skill-stocktake` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when auditing Claude skills and commands for quality. Supports Quick Scan (changed skills only) and Full Stocktake modes with sequential subagent batch evaluation.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
