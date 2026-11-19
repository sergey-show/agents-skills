---
id: everything-claude-code__angular-developer
name: angular-developer
version: 1.0.0
description: >-
  Generates Angular code and provides architectural guidance. Trigger when creating projects, components, or services, or for best practices on reactivity (signals, linkedSignal, resource), forms, dependency injection, routing, SSR, accessibility (ARIA), animations, styling (component styles, Tailwind CSS), testing, or CLI tooling.
role: angular-developer
category: engineering
triggers:
  - angular developer
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/angular-developer/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: angular-developer
---

# angular-developer

## Role

Portable distillation of upstream skill `angular-developer` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Generates Angular code and provides architectural guidance. Trigger when creating projects, components, or services, or for best practices on reactivity (signals, linkedSignal, resource), forms, dependency injection, routing, SSR, accessibility (ARIA), animations, styling (component styles, Tailwind CSS), testing, or CLI tooling.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
