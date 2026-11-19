---
id: everything-claude-code__ecc-recipes
name: ecc-recipes
version: 1.0.0
description: >-
  Map a described workflow to the right ECC command group with run-order and stop condition, or browse all command-group recipe families read live from the commands directory. Advisory only — never executes. Use when asked which commands run a workflow, the command sequence for a task, or to list ECC pipelines; not for executing the task (route to the command itself), single-command docs (use ecc-guide), or prompt rewrites (use prompt-optimizer).
role: ecc-recipes
category: meta
triggers:
  - ecc recipes
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/ecc-recipes/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ecc-recipes
---

# ecc-recipes

## Role

Portable distillation of upstream skill `ecc-recipes` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Map a described workflow to the right ECC command group with run-order and stop condition, or browse all command-group recipe families read live from the commands directory. Advisory only — never executes. Use when asked which commands run a workflow, the command sequence for a task, or to list ECC pipelines; not for executing the task (route to the command itself), single-command docs (use ecc-guide), or prompt rewrites (use prompt-optimizer).

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
