---
id: everything-claude-code__continuous-learning-v2
name: continuous-learning-v2
version: 1.0.0
description: >-
  Instinct-based learning system that observes sessions via hooks, creates atomic instincts with confidence scoring, and evolves them into skills/commands/agents. v2.1 adds project-scoped instincts to prevent cross-project contamination. Use when capturing lessons from a session, managing instincts, or promoting them into skills, commands, or agents.
role: continuous-learning-v2
category: engineering
triggers:
  - continuous learning v2
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/continuous-learning-v2/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: continuous-learning-v2
---

# continuous-learning-v2

## Role

Portable distillation of upstream skill `continuous-learning-v2` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Instinct-based learning system that observes sessions via hooks, creates atomic instincts with confidence scoring, and evolves them into skills/commands/agents. v2.1 adds project-scoped instincts to prevent cross-project contamination. Use when capturing lessons from a session, managing instincts, or promoting them into skills, commands, or agents.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
