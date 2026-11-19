---
id: everything-claude-code__token-budget-advisor
name: token-budget-advisor
version: 1.0.0
description: >-
  Offer a choice of response depth (25%/50%/75%/100%) with token estimates before answering, then answer at that level. Use when the user asks to control response length or token budget, such as 'token budget', 'short version', 'brief answer', 'respuesta corta vs larga', 'cuántos tokens', 'ahorrar tokens', 'responde al 50%', 'dame la versión corta', 'quiero controlar cuánto usas'. Skip if depth is already set this session or 'token' means an auth/payment token.
role: token-budget-advisor
category: meta
triggers:
  - token budget advisor
capabilities_required:
  - filesystem.read
capabilities_optional:
  - search.web
sources:
  - research/everything-claude-code/skills/token-budget-advisor/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: token-budget-advisor
---

# token-budget-advisor

## Role

Portable distillation of upstream skill `token-budget-advisor` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Offer a choice of response depth (25%/50%/75%/100%) with token estimates before answering, then answer at that level. Use when the user asks to control response length or token budget, such as 'token budget', 'short version', 'brief answer', 'respuesta corta vs larga', 'cuántos tokens', 'ahorrar tokens', 'responde al 50%', 'dame la versión corta', 'quiero controlar cuánto usas'. Skip if depth is already set this session or 'token' means an auth/payment token.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
