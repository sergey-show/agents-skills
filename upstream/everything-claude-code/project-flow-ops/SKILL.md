---
id: everything-claude-code__project-flow-ops
name: project-flow-ops
version: 1.0.0
description: >-
  Operate execution flow across GitHub and Linear by triaging issues and pull requests, linking active work, and keeping GitHub public-facing while Linear remains the internal execution layer. Use when the user wants backlog control, PR triage, or GitHub-to-Linear coordination.
role: project-flow-ops
category: meta
triggers:
  - project flow ops
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
sources:
  - research/everything-claude-code/skills/project-flow-ops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: project-flow-ops
---

# project-flow-ops

## Role

Portable distillation of upstream skill `project-flow-ops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Operate execution flow across GitHub and Linear by triaging issues and pull requests, linking active work, and keeping GitHub public-facing while Linear remains the internal execution layer. Use when the user wants backlog control, PR triage, or GitHub-to-Linear coordination.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
