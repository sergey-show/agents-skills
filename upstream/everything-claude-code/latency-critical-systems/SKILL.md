---
id: everything-claude-code__latency-critical-systems
name: latency-critical-systems
version: 1.0.0
description: >-
  Optimize and verify latency-sensitive systems — realtime dashboards, market data feeds, streaming agents, execution gateways, queues, and caches — by tracking p50/p95/p99 latency, freshness age, and queue depth, mapping hot paths, and running live readbacks. Use when p95 latency, throughput, or data freshness matters.
role: latency-critical-systems
category: meta
triggers:
  - latency critical systems
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - subagent.spawn
sources:
  - research/everything-claude-code/skills/latency-critical-systems/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: latency-critical-systems
---

# latency-critical-systems

## Role

Portable distillation of upstream skill `latency-critical-systems` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Optimize and verify latency-sensitive systems — realtime dashboards, market data feeds, streaming agents, execution gateways, queues, and caches — by tracking p50/p95/p99 latency, freshness age, and queue depth, mapping hot paths, and running live readbacks. Use when p95 latency, throughput, or data freshness matters.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
