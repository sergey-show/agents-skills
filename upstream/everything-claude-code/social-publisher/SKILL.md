---
id: everything-claude-code__social-publisher
name: social-publisher
version: 1.0.0
description: >-
  Agent-driven scheduling and publishing of social media posts across 13 platforms via SocialClaw. Use when the user wants to publish to X, LinkedIn, Instagram, Facebook Pages, TikTok, Discord, Telegram, YouTube, Reddit, WordPress, or Pinterest — or when managing campaigns, uploading media, or monitoring post delivery status.
role: social-publisher
category: engineering
triggers:
  - social publisher
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/social-publisher/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: social-publisher
---

# social-publisher

## Role

Portable distillation of upstream skill `social-publisher` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Agent-driven scheduling and publishing of social media posts across 13 platforms via SocialClaw. Use when the user wants to publish to X, LinkedIn, Instagram, Facebook Pages, TikTok, Discord, Telegram, YouTube, Reddit, WordPress, or Pinterest — or when managing campaigns, uploading media, or monitoring post delivery status.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
