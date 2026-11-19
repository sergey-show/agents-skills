---
id: everything-claude-code__x-api
name: x-api
version: 1.0.0
description: >-
  X/Twitter API integration for posting tweets, threads, reading timelines, search, and analytics. Covers OAuth auth patterns, rate limits, and platform-native content posting. Use when the user wants to interact with X programmatically.
role: x-api
category: meta
triggers:
  - x api
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/.agents/skills/x-api/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: x-api
---

# x-api

## Role

Portable distillation of upstream skill `x-api` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

X/Twitter API integration for posting tweets, threads, reading timelines, search, and analytics. Covers OAuth auth patterns, rate limits, and platform-native content posting. Use when the user wants to interact with X programmatically.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
