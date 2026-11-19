---
id: gstack__pair-agent
name: pair-agent
version: 1.0.0
description: >-
  Pair a remote AI agent with your browser. Use for: pair with agent, connect remote agent. (gstack)
role: pair-agent
category: meta
triggers:
  - pair agent
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
sources:
  - research/gstack/pair-agent/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: pair-agent
---

# pair-agent

## Role

Portable distillation of upstream skill `pair-agent` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Pair a remote AI agent with your browser. Use for: pair with agent, connect remote agent. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
