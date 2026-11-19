---
id: everything-claude-code__marketing-campaign
name: marketing-campaign
version: 1.0.0
description: >-
  End-to-end marketing campaign planning and execution. Covers audience research, positioning, campaign angle definition, landing page copy, email sequences, social posts, ad copy, short-form video scripts, and content calendars. Use as the orchestration layer for multi-channel product launches. Use when planning or executing a multi-channel product launch, or producing landing page, email, social, or ad copy.
role: marketing-campaign
category: research
triggers:
  - marketing campaign
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/marketing-campaign/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: marketing-campaign
---

# marketing-campaign

## Role

Portable distillation of upstream skill `marketing-campaign` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

End-to-end marketing campaign planning and execution. Covers audience research, positioning, campaign angle definition, landing page copy, email sequences, social posts, ad copy, short-form video scripts, and content calendars. Use as the orchestration layer for multi-channel product launches. Use when planning or executing a multi-channel product launch, or producing landing page, email, social, or ad copy.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
