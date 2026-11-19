---
id: everything-claude-code__agent-sort
name: agent-sort
version: 1.0.0
description: >-
  Build an evidence-backed ECC install plan for a specific repo by sorting skills, commands, rules, hooks, and extras into DAILY vs LIBRARY buckets using parallel repo-aware review passes. Use when ECC should be trimmed to what a project actually needs instead of loading the full bundle.
role: agent-sort
category: meta
triggers:
  - agent sort
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/agent-sort/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agent-sort
---

# agent-sort

## Role

Portable distillation of upstream skill `agent-sort` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build an evidence-backed ECC install plan for a specific repo by sorting skills, commands, rules, hooks, and extras into DAILY vs LIBRARY buckets using parallel repo-aware review passes. Use when ECC should be trimmed to what a project actually needs instead of loading the full bundle.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
