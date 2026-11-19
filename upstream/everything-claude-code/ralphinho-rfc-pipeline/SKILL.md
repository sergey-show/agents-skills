---
id: everything-claude-code__ralphinho-rfc-pipeline
name: ralphinho-rfc-pipeline
version: 1.0.0
description: >-
  Split an RFC into a multi-agent execution DAG — decompose into work units with dependencies and acceptance tests, run research, plan, implement, test, and review per unit, then merge through a queue with re-based branches and final system verification. Use when a feature is too large for a single agent pass, orchestrating RFC-driven multi-agent execution, or managing merge queues across agent-built units.
role: ralphinho-rfc-pipeline
category: meta
triggers:
  - ralphinho rfc pipeline
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - test.run
sources:
  - research/everything-claude-code/skills/ralphinho-rfc-pipeline/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ralphinho-rfc-pipeline
---

# ralphinho-rfc-pipeline

## Role

Portable distillation of upstream skill `ralphinho-rfc-pipeline` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Split an RFC into a multi-agent execution DAG — decompose into work units with dependencies and acceptance tests, run research, plan, implement, test, and review per unit, then merge through a queue with re-based branches and final system verification. Use when a feature is too large for a single agent pass, orchestrating RFC-driven multi-agent execution, or managing merge queues across agent-built units.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
