---
id: everything-claude-code__nextjs-turbopack
name: nextjs-turbopack
version: 1.0.0
description: >-
  Next.js 16+ and Turbopack — incremental bundling, FS caching, dev speed, and when to use Turbopack vs webpack.
role: nextjs-turbopack
category: engineering
triggers:
  - nextjs turbopack
capabilities_required:
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/.agents/skills/nextjs-turbopack/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: nextjs-turbopack
---

# nextjs-turbopack

## Role

Portable distillation of upstream skill `nextjs-turbopack` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Next.js 16+ and Turbopack — incremental bundling, FS caching, dev speed, and when to use Turbopack vs webpack.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
