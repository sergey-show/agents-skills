---
id: everything-claude-code__prompt-optimizer
name: prompt-optimizer
version: 1.0.0
description: >-
  Analyze draft prompts, detect intent and missing context, match ECC commands, skills, and agents, and output a ready-to-paste optimized prompt with diagnosis and rationale — advisory only, never executes the task. Use when the user says 'optimize prompt', 'improve my prompt', 'rewrite this prompt', 'help me prompt', 优化prompt, 改进prompt, 怎么写prompt, or 帮我优化这个指令; not for requests to optimize code or performance.
role: prompt-optimizer
category: engineering
triggers:
  - prompt optimizer
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/prompt-optimizer/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: prompt-optimizer
---

# prompt-optimizer

## Role

Portable distillation of upstream skill `prompt-optimizer` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Analyze draft prompts, detect intent and missing context, match ECC commands, skills, and agents, and output a ready-to-paste optimized prompt with diagnosis and rationale — advisory only, never executes the task. Use when the user says 'optimize prompt', 'improve my prompt', 'rewrite this prompt', 'help me prompt', 优化prompt, 改进prompt, 怎么写prompt, or 帮我优化这个指令; not for requests to optimize code or performance.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
