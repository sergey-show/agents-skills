---
id: everything-claude-code__deepseek-harness-setup
name: deepseek-harness-setup
version: 1.0.0
description: >-
  Install and operate Everything the coding agent (ECC) on the DeepSeek Harness (DSH): native skill roots (~/.dsh/skills, .agents/skills), the @deepseek-ai/dsh-hooks-claude-code bridge for command hooks, bare-insert patch mounting, generator usage, event-support limits, and update workflow. Use when setting up ECC on DeepSeek Harness, wiring ECC hooks into a DSH profile, or debugging why ECC skills or hooks do not appear in a DSH session.
role: deepseek-harness-setup
category: meta
triggers:
  - deepseek harness setup
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/deepseek-harness-setup/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: deepseek-harness-setup
---

# deepseek-harness-setup

## Role

Portable distillation of upstream skill `deepseek-harness-setup` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Install and operate Everything the coding agent (ECC) on the DeepSeek Harness (DSH): native skill roots (~/.dsh/skills, .agents/skills), the @deepseek-ai/dsh-hooks-claude-code bridge for command hooks, bare-insert patch mounting, generator usage, event-support limits, and update workflow. Use when setting up ECC on DeepSeek Harness, wiring ECC hooks into a DSH profile, or debugging why ECC skills or hooks do not appear in a DSH session.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
