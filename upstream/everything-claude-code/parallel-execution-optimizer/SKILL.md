---
id: everything-claude-code__parallel-execution-optimizer
name: parallel-execution-optimizer
version: 1.0.0
description: >-
  Speed up a task by turning it into a dependency graph of parallel lanes with a lane matrix, batched reads and checks, write surfaces isolated by file, worktree, branch, or service, and a final verification table. Use when the user wants a task done much faster through parallel work, concurrent agents, batched tool calls, isolated worktrees, many independent verification lanes, or bounded homogeneous work that reuses shared preparation while record operations remain sequential, without losing correctness.
role: parallel-execution-optimizer
category: ops
triggers:
  - parallel execution optimizer
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
  - research/everything-claude-code/skills/parallel-execution-optimizer/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: parallel-execution-optimizer
---

# parallel-execution-optimizer

## Role

Portable distillation of upstream skill `parallel-execution-optimizer` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Speed up a task by turning it into a dependency graph of parallel lanes with a lane matrix, batched reads and checks, write surfaces isolated by file, worktree, branch, or service, and a final verification table. Use when the user wants a task done much faster through parallel work, concurrent agents, batched tool calls, isolated worktrees, many independent verification lanes, or bounded homogeneous work that reuses shared preparation while record operations remain sequential, without losing correctness.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
