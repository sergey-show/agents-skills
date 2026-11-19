---
id: everything-claude-code__fal-ai-media
name: fal-ai-media
version: 1.0.0
description: >-
  Unified media generation via fal.ai MCP — image, video, and audio. Covers text-to-image (Nano Banana), text/image-to-video (Seedance, Kling, Veo 3), text-to-speech (CSM-1B), and video-to-audio (ThinkSound). Use when the user wants to generate images, videos, or audio with AI.
role: fal-ai-media
category: engineering
triggers:
  - fal ai media
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/.agents/skills/fal-ai-media/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: fal-ai-media
---

# fal-ai-media

## Role

Portable distillation of upstream skill `fal-ai-media` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Unified media generation via fal.ai MCP — image, video, and audio. Covers text-to-image (Nano Banana), text/image-to-video (Seedance, Kling, Veo 3), text-to-speech (CSM-1B), and video-to-audio (ThinkSound). Use when the user wants to generate images, videos, or audio with AI.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
