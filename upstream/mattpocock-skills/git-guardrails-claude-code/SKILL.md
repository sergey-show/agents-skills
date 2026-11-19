---
id: mattpocock-skills__git-guardrails-claude-code
name: git-guardrails-claude-code
version: 1.0.0
description: >-
  Set up the coding agent hooks to block dangerous git commands (push, reset --hard, clean, branch -D, etc.) before they execute. Use when user wants to prevent destructive git operations, add git safety hooks, or block git push/reset in the coding agent.
role: git-guardrails-claude-code
category: engineering
triggers:
  - git guardrails claude code
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/skills/skills/misc/git-guardrails-claude-code/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: git-guardrails-claude-code
---

# git-guardrails-claude-code

## Role

Portable distillation of upstream skill `git-guardrails-claude-code` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Set up the coding agent hooks to block dangerous git commands (push, reset --hard, clean, branch -D, etc.) before they execute. Use when user wants to prevent destructive git operations, add git safety hooks, or block git push/reset in the coding agent.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
