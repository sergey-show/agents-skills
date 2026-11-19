---
id: everything-claude-code__code-tour
name: code-tour
version: 1.0.0
description: >-
  Create CodeTour `.tour` files — persona-targeted, step-by-step walkthroughs with real file and line anchors. Use for onboarding tours, architecture walkthroughs, PR tours, RCA tours, and structured "explain how this works" requests. Use when the user asks for a code tour, onboarding walkthrough, PR tour, or an explanation of how a subsystem works.
role: code-tour
category: meta
triggers:
  - code tour
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
sources:
  - research/everything-claude-code/skills/code-tour/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: code-tour
---

# code-tour

## Role

Portable distillation of upstream skill `code-tour` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Create CodeTour `.tour` files — persona-targeted, step-by-step walkthroughs with real file and line anchors. Use for onboarding tours, architecture walkthroughs, PR tours, RCA tours, and structured "explain how this works" requests. Use when the user asks for a code tour, onboarding walkthrough, PR tour, or an explanation of how a subsystem works.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
