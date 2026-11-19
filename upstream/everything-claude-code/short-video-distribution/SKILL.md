---
id: everything-claude-code__short-video-distribution
name: short-video-distribution
version: 1.0.0
description: >-
  Ship a finished vertical video to TikTok, YouTube Shorts, and Instagram Reels. Checks the file against each platform's limits, writes native captions and titles, handles privacy and disclosure choices, gets explicit approval, then publishes through whichever path the user has (a connected publishing MCP server, the platform APIs, or a manual upload sheet) and returns the live links. Use after a video is rendered or edited and the user wants it posted as a Short, Reel, or TikTok.
role: short-video-distribution
category: meta
triggers:
  - short video distribution
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/short-video-distribution/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: short-video-distribution
---

# short-video-distribution

## Role

Portable distillation of upstream skill `short-video-distribution` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Ship a finished vertical video to TikTok, YouTube Shorts, and Instagram Reels. Checks the file against each platform's limits, writes native captions and titles, handles privacy and disclosure choices, gets explicit approval, then publishes through whichever path the user has (a connected publishing MCP server, the platform APIs, or a manual upload sheet) and returns the live links. Use after a video is rendered or edited and the user wants it posted as a Short, Reel, or TikTok.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
