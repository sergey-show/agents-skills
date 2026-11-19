---
id: everything-claude-code__content-engine
name: content-engine
version: 1.0.0
description: >-
  Create platform-native content systems for X, LinkedIn, TikTok, YouTube, newsletters, and repurposed multi-platform campaigns. Use when the user wants social posts, threads, scripts, content calendars, or one source asset adapted cleanly across platforms.
role: content-engine
category: engineering
triggers:
  - content engine
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
sources:
  - research/everything-claude-code/.agents/skills/content-engine/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: content-engine
---

# content-engine

## Role

Portable distillation of upstream skill `content-engine` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Create platform-native content systems for X, LinkedIn, TikTok, YouTube, newsletters, and repurposed multi-platform campaigns. Use when the user wants social posts, threads, scripts, content calendars, or one source asset adapted cleanly across platforms.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
