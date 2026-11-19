---
id: everything-claude-code__token-card
name: token-card
version: 1.0.0
description: >-
  Render a token-usage stat card from local the coding agent, Codex, Gemini CLI, and OpenCode session logs and commit it into the repository as a file. Use when someone wants a current usage figure in a README, or asks for a shareable card of their coding-agent activity.
role: token-card
category: meta
triggers:
  - token card
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/token-card/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: token-card
---

# token-card

## Role

Portable distillation of upstream skill `token-card` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Render a token-usage stat card from local the coding agent, Codex, Gemini CLI, and OpenCode session logs and commit it into the repository as a file. Use when someone wants a current usage figure in a README, or asks for a shareable card of their coding-agent activity.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
