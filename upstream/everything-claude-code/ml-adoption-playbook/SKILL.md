---
id: everything-claude-code__ml-adoption-playbook
name: ml-adoption-playbook
version: 1.0.0
description: >-
  End-to-end methodology for AI agents and software engineers to add machine learning algorithms to existing non-ML codebases. Covers problem framing, data readiness, architectural decoupling, and baseline model integration. Use when adding a machine learning capability to a codebase that has none, from problem framing through a baseline model.
role: ml-adoption-playbook
category: research
triggers:
  - ml adoption playbook
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/ml-adoption-playbook/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ml-adoption-playbook
---

# ml-adoption-playbook

## Role

Portable distillation of upstream skill `ml-adoption-playbook` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

End-to-end methodology for AI agents and software engineers to add machine learning algorithms to existing non-ML codebases. Covers problem framing, data readiness, architectural decoupling, and baseline model integration. Use when adding a machine learning capability to a codebase that has none, from problem framing through a baseline model.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
