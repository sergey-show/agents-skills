---
id: everything-claude-code__frontend-slides
name: frontend-slides
version: 1.0.0
description: >-
  Create stunning, animation-rich HTML presentations from scratch or by converting PowerPoint files. Use when the user wants to build a presentation, convert a PPT/PPTX to web, or create slides for a talk/pitch. Helps non-designers discover their aesthetic through visual exploration rather than abstract choices.
role: frontend-slides
category: engineering
triggers:
  - frontend slides
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - search.web
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/frontend-slides/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: frontend-slides
---

# frontend-slides

## Role

Portable distillation of upstream skill `frontend-slides` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Create stunning, animation-rich HTML presentations from scratch or by converting PowerPoint files. Use when the user wants to build a presentation, convert a PPT/PPTX to web, or create slides for a talk/pitch. Helps non-designers discover their aesthetic through visual exploration rather than abstract choices.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
