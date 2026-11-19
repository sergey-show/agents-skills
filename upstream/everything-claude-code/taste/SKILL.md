---
id: everything-claude-code__taste
name: taste
version: 1.0.0
description: >-
  Creative-direction layer for music videos and short-form edits in the angelcore / cloud-trance / hyperpop family — a named-genre aesthetic vocabulary, mood + color + light system, beat-synced editing grammar, and a pipeline chaining ECC's video skills from b-roll generation to distribution. Use when a video must feel intentional rather than merely functional — music videos, fancams, moodboard-driven reels, or giving AI-generated b-roll a coherent visual direction.
role: taste
category: meta
triggers:
  - taste
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/taste/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: taste
---

# taste

## Role

Portable distillation of upstream skill `taste` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Creative-direction layer for music videos and short-form edits in the angelcore / cloud-trance / hyperpop family — a named-genre aesthetic vocabulary, mood + color + light system, beat-synced editing grammar, and a pipeline chaining ECC's video skills from b-roll generation to distribution. Use when a video must feel intentional rather than merely functional — music videos, fancams, moodboard-driven reels, or giving AI-generated b-roll a coherent visual direction.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
