---
id: stitch-skills__upload-to-stitch
name: stitch::upload-to-stitch
version: 1.0.0
description: >-
  Upload local assets (images, mockups, extracted HTML, design markdown) to a Stitch project. ALWAYS use this skill when you need to upload visual assets, HTML pages, or design docs to Stitch, particularly when direct MCP tool calls fail or truncate due to base64 token limits.
role: stitch::upload-to-stitch
category: design
triggers:
  - upload to stitch
capabilities_required:
  - filesystem.read
capabilities_optional:
  - ask_user
  - search.web
  - shell.exec
sources:
  - research/stitch-skills/plugins/stitch-design/skills/upload-to-stitch/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: upload-to-stitch
---

# stitch::upload-to-stitch

## Role

Portable distillation of upstream skill `upload-to-stitch` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Upload local assets (images, mockups, extracted HTML, design markdown) to a Stitch project. ALWAYS use this skill when you need to upload visual assets, HTML pages, or design docs to Stitch, particularly when direct MCP tool calls fail or truncate due to base64 token limits.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
