---
id: everything-claude-code__roundhouse-x402
name: roundhouse-x402
version: 1.0.0
description: >-
  Discover x402-paid services and ERC-8004 agent identity via Roundhouse (open catalog, paid SQL, MCP server, rh-x402 CLI), and optionally settle through Roundhouse's Base mainnet facilitator. Use when searching the x402 bazaar/index, vetting a payee or wallet, querying settlement or agent data, configuring Roundhouse MCP, or pointing a paywall at a hosted facilitator on Base.
role: roundhouse-x402
category: meta
triggers:
  - roundhouse x402
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/roundhouse-x402/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: roundhouse-x402
---

# roundhouse-x402

## Role

Portable distillation of upstream skill `roundhouse-x402` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Discover x402-paid services and ERC-8004 agent identity via Roundhouse (open catalog, paid SQL, MCP server, rh-x402 CLI), and optionally settle through Roundhouse's Base mainnet facilitator. Use when searching the x402 bazaar/index, vetting a payee or wallet, querying settlement or agent data, configuring Roundhouse MCP, or pointing a paywall at a hosted facilitator on Base.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
