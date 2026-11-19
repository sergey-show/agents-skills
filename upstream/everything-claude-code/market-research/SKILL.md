---
id: everything-claude-code__market-research
name: market-research
version: 1.0.0
description: >-
  Conduct market research, competitive analysis, investor due diligence, and industry intelligence with source attribution and decision-oriented summaries. Use when the user wants market sizing, competitor comparisons, fund research, technology scans, or research that informs business decisions.
role: market-research
category: research
triggers:
  - market research
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/market-research/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: market-research
---

# market-research

## Role

Portable distillation of upstream skill `market-research` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Conduct market research, competitive analysis, investor due diligence, and industry intelligence with source attribution and decision-oriented summaries. Use when the user wants market sizing, competitor comparisons, fund research, technology scans, or research that informs business decisions.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
