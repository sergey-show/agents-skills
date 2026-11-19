---
id: mattpocock-skills__writing-for-agents
name: writing-for-agents
version: 1.0.0
description: >-
  Writing documents for agents. Use when creating or editing skills, or modifying AGENTS.md or CLAUDE.md.
role: writing-for-agents
category: research
triggers:
  - writing for agents
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/skills/skills/productivity/writing-for-agents/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: writing-for-agents
---

# writing-for-agents

## Role

Portable distillation of upstream skill `writing-for-agents` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Writing documents for agents. Use when creating or editing skills, or modifying AGENTS.md or CLAUDE.md.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
