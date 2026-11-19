---
id: everything-claude-code__brand-voice
name: brand-voice
version: 1.0.0
description: >-
  Build a source-derived writing style profile from real posts, essays, launch notes, docs, or site copy, then reuse that profile across content, outreach, and social workflows. Use when the user wants voice consistency without generic AI writing tropes.
role: brand-voice
category: research
triggers:
  - brand voice
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/brand-voice/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: brand-voice
---

# brand-voice

## Role

Portable distillation of upstream skill `brand-voice` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build a source-derived writing style profile from real posts, essays, launch notes, docs, or site copy, then reuse that profile across content, outreach, and social workflows. Use when the user wants voice consistency without generic AI writing tropes.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
