---
id: superpowers__finishing-a-development-branch
name: finishing-a-development-branch
version: 1.0.0
description: >-
  Use when implementation is complete, all tests pass, and you need to decide how to integrate the work
role: finishing-a-development-branch
category: meta
triggers:
  - finishing a development branch
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/superpowers/skills/finishing-a-development-branch/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: finishing-a-development-branch
---

# finishing-a-development-branch

## Role

Portable distillation of upstream skill `finishing-a-development-branch` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when implementation is complete, all tests pass, and you need to decide how to integrate the work

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
