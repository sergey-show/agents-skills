---
id: everything-claude-code__enterprise-agent-ops
name: enterprise-agent-ops
version: 1.0.0
description: >-
  Operational controls for long-lived or cloud-hosted agent systems — runtime lifecycle (start, pause, stop, restart), observability (logs, metrics, traces), least-privilege safety scopes and kill switches, and rollout/rollback change management with audit logs and success/cost metrics. Use when running production agent fleets on PM2, systemd, or containers that need monitoring, incident response, or deployment gates.
role: enterprise-agent-ops
category: ops
triggers:
  - enterprise agent ops
capabilities_required:
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/enterprise-agent-ops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: enterprise-agent-ops
---

# enterprise-agent-ops

## Role

Portable distillation of upstream skill `enterprise-agent-ops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Operational controls for long-lived or cloud-hosted agent systems — runtime lifecycle (start, pause, stop, restart), observability (logs, metrics, traces), least-privilege safety scopes and kill switches, and rollout/rollback change management with audit logs and success/cost metrics. Use when running production agent fleets on PM2, systemd, or containers that need monitoring, incident response, or deployment gates.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
