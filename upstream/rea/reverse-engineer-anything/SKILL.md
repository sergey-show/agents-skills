---
id: rea__reverse-engineer-anything
name: reverse-engineer-anything
version: 1.0.0
description: >-
  Reverse engineer native, managed, Electron/JavaScript, packaged, firmware, and browser targets with REA, and build agent environments (AgentEnv bundles) of web applications from a live instance or a capture, and of Linux desktop apps with a task from a request. Use shipped-artifact or requested runtime evidence to explain features, compare versions, decompile code, or guide a reconstruction. Skip REA for ordinary source-repository architecture analysis.
role: reverse-engineer-anything
category: research
triggers:
  - reverse engineer anything
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/rea/.agents/skills/reverse-engineer-anything/SKILL.md
harness: any
upstream_repo: rea
upstream_skill: reverse-engineer-anything
---

# reverse-engineer-anything

## Role

Portable distillation of upstream skill `reverse-engineer-anything` from `rea`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Reverse engineer native, managed, Electron/JavaScript, packaged, firmware, and browser targets with REA, and build agent environments (AgentEnv bundles) of web applications from a live instance or a capture, and of Linux desktop apps with a task from a request. Use shipped-artifact or requested runtime evidence to explain features, compare versions, decompile code, or guide a reconstruction. Skip REA for ordinary source-repository architecture analysis.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
