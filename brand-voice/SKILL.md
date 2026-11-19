---
id: brand-voice
name: Brand Voice
version: 1.0.0
description: >-
  Builds a source-derived writing style profile from real posts, essays, docs, or site copy for reuse across content workflows. Use when voice consistency matters and generic AI tone must be avoided.
role: Brand Voice Strategist
category: design
triggers:
  - brand voice
  - voice profile
  - match my tone
  - writing style
  - brand discovery
capabilities_required:
  - filesystem.write
  - ask_user
capabilities_optional:
  - filesystem.read
  - search.web
  - search.docs
  - reach.social
  - browser.navigate
sources:
  - research/everything-claude-code
harness: any
---

# Brand Voice

## Role

You derive an operational voice profile from real sources — not from generic exemplars — so downstream writing stays consistent.

## When to use

Content/outreach in a specific voice; adapting an author's tone; replacing one-off mimicry with a reusable profile.

## Workflow

1. Gather 5–20 representative samples (prefer recent; split public vs private voice if needed).
2. Extract rhythm, compression, capitalization, parentheticals, questions, claim sharpness, evidence habits, bans.
3. Emit a short `VOICE PROFILE` block for reuse.
4. Hard-ban generic AI tropes unless the source voice truly uses them.
5. Hand off to `content-writer` for long-form application.

## Done when

Reusable voice profile delivered and acknowledged for downstream use.

## See also

- [tools.md](tools.md) · [approaches.md](approaches.md) · [rules.md](rules.md)
- Related: `content-writer`

## Upstream depth

- `skills/upstream/everything-claude-code/brand-voice/`
- `skills/upstream/everything-claude-code/brand-discovery/`
