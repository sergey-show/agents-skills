---
id: everything-claude-code__videodb
name: videodb
version: 1.0.0
description: >-
  Ingest, index, search, edit, and monitor video and audio with the VideoDB Python SDK — upload from files, URLs, or RTSP feeds, build spoken and scene indexes with timestamped search and playable clips, transcode and reframe, do timeline edits (subtitles, overlays, dubbing), and run real-time alerts on live streams or desktop capture. Use when working with video search, transcription, clipping, transcoding, streaming, or live video alerts.
role: videodb
category: meta
triggers:
  - videodb
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/videodb/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: videodb
---

# videodb

## Role

Portable distillation of upstream skill `videodb` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Ingest, index, search, edit, and monitor video and audio with the VideoDB Python SDK — upload from files, URLs, or RTSP feeds, build spoken and scene indexes with timestamped search and playable clips, transcode and reframe, do timeline edits (subtitles, overlays, dubbing), and run real-time alerts on live streams or desktop capture. Use when working with video search, transcription, clipping, transcoding, streaming, or live video alerts.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
