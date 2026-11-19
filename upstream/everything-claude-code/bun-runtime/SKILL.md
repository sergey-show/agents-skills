---
id: everything-claude-code__bun-runtime
name: bun-runtime
version: 1.0.0
description: >-
  Bun as runtime, package manager, bundler, and test runner. When to choose Bun vs Node, migration notes, and Vercel support.
role: bun-runtime
category: ops
triggers:
  - bun runtime
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/bun-runtime/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: bun-runtime
---

# bun-runtime

## Role

Portable distillation of upstream skill `bun-runtime` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Bun as runtime, package manager, bundler, and test runner. When to choose Bun vs Node, migration notes, and Vercel support.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
