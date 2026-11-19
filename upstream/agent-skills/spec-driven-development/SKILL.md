---
id: agent-skills__spec-driven-development
name: spec-driven-development
version: 1.0.0
description: >-
  Creates specs before coding. Use when starting a new project, feature, or significant change and no specification exists yet. Use when drafting a PRD or requirements document with objectives and scope, or when requirements are unclear, ambiguous, or only exist as a vague idea. Use when a single requirement spans several independently testable capabilities and needs decomposing into a capability map of modules before specifying. Use when evolving a shipped spec — scoping a V1, deferring ideas to a V2 backlog, or writing a follow-up spec for a change to an existing feature.
role: spec-driven-development
category: engineering
triggers:
  - spec driven development
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/spec-driven-development/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: spec-driven-development
---

# spec-driven-development

## Role

Portable distillation of upstream skill `spec-driven-development` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Creates specs before coding. Use when starting a new project, feature, or significant change and no specification exists yet. Use when drafting a PRD or requirements document with objectives and scope, or when requirements are unclear, ambiguous, or only exist as a vague idea. Use when a single requirement spans several independently testable capabilities and needs decomposing into a capability map of modules before specifying. Use when evolving a shipped spec — scoping a V1, deferring ideas to a V2 backlog, or writing a follow-up spec for a change to an existing feature.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
