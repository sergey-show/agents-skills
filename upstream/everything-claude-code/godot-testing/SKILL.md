---
id: everything-claude-code__godot-testing
name: godot-testing
version: 1.0.0
description: >-
  Testing Godot 4 GDScript projects - a zero-dependency headless check scene, gdUnit4 and GUT suites, scene-runner tests, signal assertions, and CI commands. Use when adding tests to a Godot project, setting up CI, or proving a change did not break the game.
role: godot-testing
category: engineering
triggers:
  - godot testing
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/godot-testing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: godot-testing
---

# godot-testing

## Role

Portable distillation of upstream skill `godot-testing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Testing Godot 4 GDScript projects - a zero-dependency headless check scene, gdUnit4 and GUT suites, scene-runner tests, signal assertions, and CI commands. Use when adding tests to a Godot project, setting up CI, or proving a change did not break the game.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
