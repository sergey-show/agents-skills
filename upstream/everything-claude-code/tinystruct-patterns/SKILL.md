---
id: everything-claude-code__tinystruct-patterns
name: tinystruct-patterns
version: 1.0.0
description: >-
  Expert guidance for developing with the tinystruct Java framework. Use when working on the tinystruct codebase or any project built on tinystruct — including generating the bin/dispatcher and bin/dispatcher.cmd launcher scripts when a project lacks them, creating Application classes, @Action-mapped routes, unit tests, ActionRegistry, HTTP/CLI dual-mode handling, the built-in HTTP server, the event system, JSON with Builder/Builders, database persistence with AbstractData, POJO generation, Server-Sent Events (SSE), file uploads, and outbound HTTP networking.
role: tinystruct-patterns
category: engineering
triggers:
  - tinystruct patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/tinystruct-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: tinystruct-patterns
---

# tinystruct-patterns

## Role

Portable distillation of upstream skill `tinystruct-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Expert guidance for developing with the tinystruct Java framework. Use when working on the tinystruct codebase or any project built on tinystruct — including generating the bin/dispatcher and bin/dispatcher.cmd launcher scripts when a project lacks them, creating Application classes, @Action-mapped routes, unit tests, ActionRegistry, HTTP/CLI dual-mode handling, the built-in HTTP server, the event system, JSON with Builder/Builders, database persistence with AbstractData, POJO generation, Server-Sent Events (SSE), file uploads, and outbound HTTP networking.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
