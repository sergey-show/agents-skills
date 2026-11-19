---
id: agent-skills__observability-and-instrumentation
name: observability-and-instrumentation
version: 1.0.0
description: >-
  Instruments code so production behavior is visible and diagnosable. Use when adding logging, metrics, tracing, or alerting. Use when shipping any feature that runs in production and you need evidence it works. Use when production issues are reported but you can't tell what happened from the available data.
role: observability-and-instrumentation
category: ops
triggers:
  - observability and instrumentation
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/agent-skills/skills/observability-and-instrumentation/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: observability-and-instrumentation
---

# observability-and-instrumentation

## Role

Portable distillation of upstream skill `observability-and-instrumentation` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Instruments code so production behavior is visible and diagnosable. Use when adding logging, metrics, tracing, or alerting. Use when shipping any feature that runs in production and you need evidence it works. Use when production issues are reported but you can't tell what happened from the available data.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
