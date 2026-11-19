---
id: everything-claude-code__codehealth-mcp
name: codehealth-mcp
version: 1.0.0
description: >-
  Real-time structural Code Health via CodeScene MCP — review before edits, verify score deltas after changes, gate commits and PRs. Use when reviewing code quality, refactoring, checking if AI changes degraded a file, or before commit/PR.
role: codehealth-mcp
category: design
triggers:
  - codehealth mcp
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/codehealth-mcp/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: codehealth-mcp
---

# codehealth-mcp

## Role

Portable distillation of upstream skill `codehealth-mcp` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Real-time structural Code Health via CodeScene MCP — review before edits, verify score deltas after changes, gate commits and PRs. Use when reviewing code quality, refactoring, checking if AI changes degraded a file, or before commit/PR.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
