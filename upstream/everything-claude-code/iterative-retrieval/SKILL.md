---
id: everything-claude-code__iterative-retrieval
name: iterative-retrieval
version: 1.0.0
description: >-
  Pattern for progressively refining context retrieval to solve the subagent context problem. Use when a subagent lacks the context it needs and retrieval must be refined across passes.
role: iterative-retrieval
category: design
triggers:
  - iterative retrieval
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/iterative-retrieval/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: iterative-retrieval
---

# iterative-retrieval

## Role

Portable distillation of upstream skill `iterative-retrieval` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Pattern for progressively refining context retrieval to solve the subagent context problem. Use when a subagent lacks the context it needs and retrieval must be refined across passes.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
