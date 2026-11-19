---
id: everything-claude-code__investor-outreach
name: investor-outreach
version: 1.0.0
description: >-
  Draft cold emails, warm intro blurbs, follow-ups, update emails, and investor communications for fundraising. Use when the user wants outreach to angels, VCs, strategic investors, or accelerators and needs concise, personalized, investor-facing messaging.
role: investor-outreach
category: research
triggers:
  - investor outreach
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/.agents/skills/investor-outreach/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: investor-outreach
---

# investor-outreach

## Role

Portable distillation of upstream skill `investor-outreach` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Draft cold emails, warm intro blurbs, follow-ups, update emails, and investor communications for fundraising. Use when the user wants outreach to angels, VCs, strategic investors, or accelerators and needs concise, personalized, investor-facing messaging.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
