---
id: everything-claude-code__agent-eval
name: agent-eval
version: 1.0.0
description: >-
  Head-to-head comparison of coding agents (the coding agent, Aider, Codex, etc.) on custom tasks with pass rate, cost, time, and consistency metrics. Use when choosing between coding agents, or when a change to an agent setup needs measured pass rate, cost, and time rather than an impression.
role: agent-eval
category: meta
triggers:
  - agent eval
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/agent-eval/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agent-eval
---

# agent-eval

## Role

Portable distillation of upstream skill `agent-eval` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Head-to-head comparison of coding agents (the coding agent, Aider, Codex, etc.) on custom tasks with pass rate, cost, time, and consistency metrics. Use when choosing between coding agents, or when a change to an agent setup needs measured pass rate, cost, and time rather than an impression.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
