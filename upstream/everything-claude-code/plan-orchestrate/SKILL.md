---
id: everything-claude-code__plan-orchestrate
name: plan-orchestrate
version: 1.0.0
description: >-
  Read a plan document, decompose it into steps, classify each step, and emit the ready-to-paste ECC slash command for that step, carrying the step identifier and scope in the command's own documented argument form. Generative only — never invokes commands itself and never claims to control what a command runs internally. Steps whose command cannot carry plan scope fail closed instead of being emitted. Use when the user has a multi-step plan and wants the right command for each step without picking it by hand.
role: plan-orchestrate
category: meta
triggers:
  - plan orchestrate
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
  - research/everything-claude-code/skills/plan-orchestrate/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: plan-orchestrate
---

# plan-orchestrate

## Role

Portable distillation of upstream skill `plan-orchestrate` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Read a plan document, decompose it into steps, classify each step, and emit the ready-to-paste ECC slash command for that step, carrying the step identifier and scope in the command's own documented argument form. Generative only — never invokes commands itself and never claims to control what a command runs internally. Steps whose command cannot carry plan scope fail closed instead of being emitted. Use when the user has a multi-step plan and wants the right command for each step without picking it by hand.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
