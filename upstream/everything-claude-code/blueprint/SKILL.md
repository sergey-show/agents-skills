---
id: everything-claude-code__blueprint
name: blueprint
version: 1.0.0
description: >-
  Turn a one-line objective into a step-by-step construction plan for multi-session, multi-agent engineering projects: one-PR-sized steps with self-contained context briefs, dependency graph with parallel-step detection, adversarial review gate, and plan mutation protocol. Use when planning a large feature, refactor, or roadmap that spans multiple PRs or sessions; not for single-PR tasks or when the user says \"just do it\".
role: blueprint
category: engineering
triggers:
  - blueprint
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/blueprint/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: blueprint
---

# blueprint

## Role

Portable distillation of upstream skill `blueprint` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Turn a one-line objective into a step-by-step construction plan for multi-session, multi-agent engineering projects: one-PR-sized steps with self-contained context briefs, dependency graph with parallel-step detection, adversarial review gate, and plan mutation protocol. Use when planning a large feature, refactor, or roadmap that spans multiple PRs or sessions; not for single-PR tasks or when the user says \"just do it\".

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
