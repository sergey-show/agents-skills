---
id: everything-claude-code__codebase-onboarding
name: codebase-onboarding
version: 1.0.0
description: >-
  Analyze an unfamiliar codebase and generate a structured onboarding guide with architecture map, key entry points, conventions, and a starter CLAUDE.md. Use when joining a new project or setting up the coding agent for the first time in a repo.
role: codebase-onboarding
category: design
triggers:
  - codebase onboarding
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/codebase-onboarding/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: codebase-onboarding
---

# codebase-onboarding

## Role

Portable distillation of upstream skill `codebase-onboarding` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Analyze an unfamiliar codebase and generate a structured onboarding guide with architecture map, key entry points, conventions, and a starter CLAUDE.md. Use when joining a new project or setting up the coding agent for the first time in a repo.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
