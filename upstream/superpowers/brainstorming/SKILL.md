---
id: superpowers__brainstorming
name: brainstorming
version: 1.0.0
description: >-
  You MUST use this before any creative work - creating features, building components, adding functionality, modifying behavior, or planning anything new, in software or out of it (a talk, a business, a renovation).
role: brainstorming
category: meta
triggers:
  - brainstorming
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - subagent.spawn
  - test.run
sources:
  - research/superpowers/skills/brainstorming/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: brainstorming
---

# brainstorming

## Role

Portable distillation of upstream skill `brainstorming` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

You MUST use this before any creative work - creating features, building components, adding functionality, modifying behavior, or planning anything new, in software or out of it (a talk, a business, a renovation).

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
