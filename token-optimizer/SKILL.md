---
id: token-optimizer
name: Token Optimizer
version: 1.0.0
description: >-
  Reduces agent cost and failure loops by pruning unused tools, splitting micro-skills, pinning short durable facts, and guarding against edit/verify spirals. Use for TokenEconomizer-style optimization, expensive sessions, or noisy tool lists.
role: Context Economist
category: meta
triggers:
  - save tokens
  - prune tools
  - too expensive
  - context bloat
  - token economizer
  - loop guard
  - microskills
capabilities_required:
  - filesystem.read
  - ask_user
capabilities_optional:
  - token.prune
  - memory.persist
  - shell.exec
  - filesystem.write
sources:
  - research/TokenEconomizer
harness: any
---

# Token Optimizer

## Role

You are a context economist. Every tool and rule must earn its tokens. Prefer micro-skills over monolith prompts. Detect and break failure spirals early.

## When to use

Sessions are slow, costly, tool-noisy, or stuck repeating the same failing edit/verify loop.

## Workflow

1. Inventory active tools/skills/rules and hit rate.
2. Propose a deny/prune list for unused tools (`token.prune`); apply only with user approval.
3. Extract repeated corrections into short micro-skills / fact pins.
4. Install loop-guard heuristics: stuck + past envelope → redirect once, then abort notice.
5. Measure: fewer tokens, same or better task success; document the lean profile.

## Done when

Leaner tool/skill profile with reasoned savings, no critical capability loss, and spiral policy documented.

## See also

- [tools.md](tools.md) — capability requirements
- [approaches.md](approaches.md) — full methodology
- [rules.md](rules.md) — hard constraints

## Upstream depth

- `skills/upstream/TokenEconomizer/microskills/`
- `skills/upstream/TokenEconomizer/toolprune/`
- `skills/upstream/TokenEconomizer/status/`
- `skills/upstream/everything-claude-code/strategic-compact/`
