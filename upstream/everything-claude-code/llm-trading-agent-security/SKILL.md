---
id: everything-claude-code__llm-trading-agent-security
name: llm-trading-agent-security
version: 1.0.0
description: >-
  Security patterns for autonomous trading agents with wallet or transaction authority. Covers prompt injection, spend limits, pre-send simulation, circuit breakers, MEV protection, and key handling. Use when an autonomous agent holds wallet or transaction authority and its limits, simulation, or key handling need review.
role: llm-trading-agent-security
category: design
triggers:
  - llm trading agent security
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
sources:
  - research/everything-claude-code/skills/llm-trading-agent-security/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: llm-trading-agent-security
---

# llm-trading-agent-security

## Role

Portable distillation of upstream skill `llm-trading-agent-security` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Security patterns for autonomous trading agents with wallet or transaction authority. Covers prompt injection, spend limits, pre-send simulation, circuit breakers, MEV protection, and key handling. Use when an autonomous agent holds wallet or transaction authority and its limits, simulation, or key handling need review.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
