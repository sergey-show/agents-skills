---
id: everything-claude-code__dmux-workflows
name: dmux-workflows
version: 1.0.0
description: >-
  Multi-agent orchestration using dmux (tmux pane manager for AI agents). Patterns for parallel agent workflows across the coding agent, Codex, OpenCode, and other harnesses. Use when running multiple agent sessions in parallel or coordinating multi-agent development workflows.
role: dmux-workflows
category: meta
triggers:
  - dmux workflows
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/dmux-workflows/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: dmux-workflows
---

# dmux-workflows

## Role

Portable distillation of upstream skill `dmux-workflows` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Multi-agent orchestration using dmux (tmux pane manager for AI agents). Patterns for parallel agent workflows across the coding agent, Codex, OpenCode, and other harnesses. Use when running multiple agent sessions in parallel or coordinating multi-agent development workflows.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
