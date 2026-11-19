---
id: everything-claude-code__brand-discovery
name: brand-discovery
version: 1.0.0
description: >-
  Use when a brand needs to discover or articulate its identity through structured multi-session interviews. Covers purpose, positioning, audience, personality, voice, narrative, and founder-brand tension across 8 modules using laddering, 5 Whys, and projective techniques. Produces a resumable session with disk-persisted state and a master brandbook (90_SYNTHESIS.md).
role: brand-discovery
category: design
triggers:
  - brand discovery
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/.agents/skills/brand-discovery/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: brand-discovery
---

# brand-discovery

## Role

Portable distillation of upstream skill `brand-discovery` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when a brand needs to discover or articulate its identity through structured multi-session interviews. Covers purpose, positioning, audience, personality, voice, narrative, and founder-brand tension across 8 modules using laddering, 5 Whys, and projective techniques. Produces a resumable session with disk-persisted state and a master brandbook (90_SYNTHESIS.md).

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
