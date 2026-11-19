---
id: everything-claude-code__verification-loop
name: verification-loop
version: 1.0.0
description: >-
  A comprehensive verification system for the coding agent sessions. Use when verifying a the coding agent session's work before claiming it is complete.
role: verification-loop
category: meta
triggers:
  - verification loop
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/verification-loop/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: verification-loop
---

# verification-loop

## Role

Portable distillation of upstream skill `verification-loop` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

A comprehensive verification system for the coding agent sessions. Use when verifying a the coding agent session's work before claiming it is complete.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
