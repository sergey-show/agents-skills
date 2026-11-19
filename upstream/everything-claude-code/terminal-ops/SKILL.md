---
id: everything-claude-code__terminal-ops
name: terminal-ops
version: 1.0.0
description: >-
  Evidence-first repo execution workflow for ECC. Use when the user wants a command run, a repo checked, a CI failure debugged, or a narrow fix pushed with exact proof of what was executed and verified.
role: terminal-ops
category: meta
triggers:
  - terminal ops
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/terminal-ops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: terminal-ops
---

# terminal-ops

## Role

Portable distillation of upstream skill `terminal-ops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Evidence-first repo execution workflow for ECC. Use when the user wants a command run, a repo checked, a CI failure debugged, or a narrow fix pushed with exact proof of what was executed and verified.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
