---
id: everything-claude-code__skill-scout
name: skill-scout
version: 1.0.0
description: >-
  Search existing local, marketplace, GitHub, and web skill sources before creating a new skill. Use when the user wants to create, build, fork, or find a skill for a workflow.
role: skill-scout
category: research
triggers:
  - skill scout
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/skill-scout/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: skill-scout
---

# skill-scout

## Role

Portable distillation of upstream skill `skill-scout` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Search existing local, marketplace, GitHub, and web skill sources before creating a new skill. Use when the user wants to create, build, fork, or find a skill for a workflow.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
