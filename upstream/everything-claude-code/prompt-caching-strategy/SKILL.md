---
id: everything-claude-code__prompt-caching-strategy
name: prompt-caching-strategy
version: 1.0.0
description: >-
  Optimize LLM prompt caching hit rate to reduce API costs and improve latency. Analyzes prompt structure, identifies cacheable vs non-cacheable content, and recommends restructuring to maximize cache reuse. TRIGGER when: user says "prompt cache", "cache hit rate", "reduce LLM cost", "optimize token usage", "cheaper LLM calls", or asks about prompt caching strategies for OpenAI/Anthropic/other providers. DO NOT TRIGGER when: user just wants to optimize a single prompt's quality (use prompt-optimizer instead), or asks about general caching infrastructure.
role: prompt-caching-strategy
category: meta
triggers:
  - prompt caching strategy
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - search.web
  - test.run
sources:
  - research/everything-claude-code/skills/prompt-caching-strategy/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: prompt-caching-strategy
---

# prompt-caching-strategy

## Role

Portable distillation of upstream skill `prompt-caching-strategy` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Optimize LLM prompt caching hit rate to reduce API costs and improve latency. Analyzes prompt structure, identifies cacheable vs non-cacheable content, and recommends restructuring to maximize cache reuse. TRIGGER when: user says "prompt cache", "cache hit rate", "reduce LLM cost", "optimize token usage", "cheaper LLM calls", or asks about prompt caching strategies for OpenAI/Anthropic/other providers. DO NOT TRIGGER when: user just wants to optimize a single prompt's quality (use prompt-optimizer instead), or asks about general caching infrastructure.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
