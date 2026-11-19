---
id: everything-claude-code__skill-comply
name: skill-comply
version: 1.0.0
description: >-
  Visualize whether skills, rules, and agent definitions are actually followed — auto-generates scenarios at 3 prompt strictness levels, runs agents, classifies behavioral sequences, and reports compliance rates with full tool call timelines. Use when checking whether agents actually follow the skills, rules, and definitions they were given, rather than assuming they do.
role: skill-comply
category: meta
triggers:
  - skill comply
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/skill-comply/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: skill-comply
---

# skill-comply

## Role

Portable distillation of upstream skill `skill-comply` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Visualize whether skills, rules, and agent definitions are actually followed — auto-generates scenarios at 3 prompt strictness levels, runs agents, classifies behavioral sequences, and reports compliance rates with full tool call timelines. Use when checking whether agents actually follow the skills, rules, and definitions they were given, rather than assuming they do.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
