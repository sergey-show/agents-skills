---
id: everything-claude-code__cost-aware-llm-pipeline
name: cost-aware-llm-pipeline
version: 1.0.0
description: >-
  Cost optimization patterns for LLM API usage — model routing by task complexity, budget tracking, retry logic, and prompt caching. Use when LLM spend needs to come down, or when routing tasks across model tiers and budgets.
role: cost-aware-llm-pipeline
category: engineering
triggers:
  - cost aware llm pipeline
capabilities_required:
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/cost-aware-llm-pipeline/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: cost-aware-llm-pipeline
---

# cost-aware-llm-pipeline

## Role

Portable distillation of upstream skill `cost-aware-llm-pipeline` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Cost optimization patterns for LLM API usage — model routing by task complexity, budget tracking, retry logic, and prompt caching. Use when LLM spend needs to come down, or when routing tasks across model tiers and budgets.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
