---
id: agent-skills__test-driven-development
name: test-driven-development
version: 1.0.0
description: >-
  Drives development with tests using the red-green-refactor loop. Use when implementing any logic, fixing any bug, or changing any behavior. Use when you need to prove that code works, when a bug report arrives, or when you're about to modify existing functionality. Use when asked to add tests to a function, fix a bug in it or change its behavior, even when the code is pasted inline, the request does not mention tests and the answer looks obvious from reading it. The skill writes the failing test first and changes the function second, never the change alone.
role: test-driven-development
category: engineering
triggers:
  - test driven development
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/agent-skills/skills/test-driven-development/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: test-driven-development
---

# test-driven-development

## Role

Portable distillation of upstream skill `test-driven-development` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Drives development with tests using the red-green-refactor loop. Use when implementing any logic, fixing any bug, or changing any behavior. Use when you need to prove that code works, when a bug report arrives, or when you're about to modify existing functionality. Use when asked to add tests to a function, fix a bug in it or change its behavior, even when the code is pasted inline, the request does not mention tests and the answer looks obvious from reading it. The skill writes the failing test first and changes the function second, never the change alone.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
