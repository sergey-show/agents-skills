---
id: everything-claude-code__agent-self-evaluation
name: agent-self-evaluation
version: 1.0.0
description: >-
  Use after completing any non-trivial task. The agent self-rates its output on 5 axes — accuracy, completeness, clarity, actionability, conciseness — with concrete evidence per criterion. Produces a structured 1-5 scorecard with specific improvement suggestions.
role: agent-self-evaluation
category: meta
triggers:
  - agent self evaluation
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/agent-self-evaluation/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agent-self-evaluation
---

# agent-self-evaluation

## Role

Portable distillation of upstream skill `agent-self-evaluation` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use after completing any non-trivial task. The agent self-rates its output on 5 axes — accuracy, completeness, clarity, actionability, conciseness — with concrete evidence per criterion. Produces a structured 1-5 scorecard with specific improvement suggestions.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
