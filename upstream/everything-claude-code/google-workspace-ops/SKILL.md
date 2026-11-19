---
id: everything-claude-code__google-workspace-ops
name: google-workspace-ops
version: 1.0.0
description: >-
  Operate across Google Drive, Docs, Sheets, and Slides as one workflow surface for plans, trackers, decks, and shared documents. Use when the user needs to find, summarize, edit, migrate, or clean up Google Workspace assets without dropping to raw tool calls.
role: google-workspace-ops
category: meta
triggers:
  - google workspace ops
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/google-workspace-ops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: google-workspace-ops
---

# google-workspace-ops

## Role

Portable distillation of upstream skill `google-workspace-ops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Operate across Google Drive, Docs, Sheets, and Slides as one workflow surface for plans, trackers, decks, and shared documents. Use when the user needs to find, summarize, edit, migrate, or clean up Google Workspace assets without dropping to raw tool calls.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
