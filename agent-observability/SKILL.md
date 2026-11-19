---
id: agent-observability
name: Agent Observability
version: 1.0.0
description: >-
  Adds or maintains local agent telemetry for tool latency, token/cost usage, session traces, and multi-agent stage attribution. Use when wiring hook-based metrics, debugging missing usage events, or auditing agent spend.
role: Agent Observability Engineer
category: meta
triggers:
  - agent observability
  - token metrics
  - session cost
  - tool latency
  - agent telemetry
  - usage events
capabilities_required:
  - filesystem.read
  - filesystem.write
capabilities_optional:
  - shell.exec
  - ask_user
  - memory.persist
sources:
  - research/LoopForge
harness: any
---

# Agent Observability

## Role

You instrument agent sessions with local, inspectable metrics — without blocking the main agent loop.

## When to use

Need tool latency, transcript token/cost, multi-agent stage attribution, or to debug missing usage events.

## Workflow

1. Agree metric sinks (NDJSON log + small state sidecar) and privacy boundaries.
2. Wire pre/post tool hooks and session start/stop emitters — command-only, short timeouts (≈5–10s).
3. Smoke-test a normal session; verify `event`, `sid`, `ts` on every line.
4. Emit `tool` (latency), `usage` (tokens/cost), `stop` (flush), optional `stage_transition` for orchestrated flows.
5. Never block or fail the main flow — hooks exit 0 even on metric errors.

## Done when

Metrics appear for a real session; schema documented; hooks non-blocking.

## See also

- [tools.md](tools.md) · [approaches.md](approaches.md) · [rules.md](rules.md)
- Related: `token-optimizer`, `orchestrator`

## Upstream depth

- `skills/upstream/everything-claude-code/agent-introspection-debugging/`
- `skills/upstream/TokenEconomizer/status/`
