---
id: mattpocock-skills__claude-handoff
name: claude-handoff
version: 1.0.0
description: >-
  Hand the current conversation off to a fresh background agent that picks up the work immediately.
role: claude-handoff
category: engineering
triggers:
  - claude handoff
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
sources:
  - research/skills/skills/in-progress/claude-handoff/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: claude-handoff
---

# claude-handoff

## Role

Portable distillation of upstream skill `claude-handoff` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Hand the current conversation off to a fresh background agent that picks up the work immediately.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
