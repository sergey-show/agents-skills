---
id: agent-skills__context-engineering
name: context-engineering
version: 1.0.0
description: >-
  Optimizes agent context setup. Use when starting a new session, when agent output quality degrades, when switching between tasks, or when you need to configure rules files and context for a project.
role: context-engineering
category: engineering
triggers:
  - context engineering
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/context-engineering/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: context-engineering
---

# context-engineering

## Role

Portable distillation of upstream skill `context-engineering` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Optimizes agent context setup. Use when starting a new session, when agent output quality degrades, when switching between tasks, or when you need to configure rules files and context for a project.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
