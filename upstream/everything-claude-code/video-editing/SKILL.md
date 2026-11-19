---
id: everything-claude-code__video-editing
name: video-editing
version: 1.0.0
description: >-
  AI-assisted video editing workflows for cutting, structuring, and augmenting real footage. Covers the full pipeline from raw capture through FFmpeg, Remotion, ElevenLabs, fal.ai, and final polish in Descript or CapCut. Use when the user wants to edit video, cut footage, create vlogs, or build video content.
role: video-editing
category: engineering
triggers:
  - video editing
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/.agents/skills/video-editing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: video-editing
---

# video-editing

## Role

Portable distillation of upstream skill `video-editing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

AI-assisted video editing workflows for cutting, structuring, and augmenting real footage. Covers the full pipeline from raw capture through FFmpeg, Remotion, ElevenLabs, fal.ai, and final polish in Descript or CapCut. Use when the user wants to edit video, cut footage, create vlogs, or build video content.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
