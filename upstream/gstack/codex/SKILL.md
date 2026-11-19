---
id: gstack__codex
name: codex
version: 1.0.0
description: >-
  OpenAI the coding agent wrapper — three modes. Use for: codex review, second opinion, outside voice challenge. (gstack)
role: codex
category: meta
triggers:
  - codex
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/codex/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: codex
---

# codex

## Role

Portable distillation of upstream skill `codex` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

OpenAI the coding agent wrapper — three modes. Use for: codex review, second opinion, outside voice challenge. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
