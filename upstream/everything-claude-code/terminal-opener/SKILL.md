---
id: everything-claude-code__terminal-opener
name: terminal-opener
version: 1.0.0
description: >-
  Open an executable and its argument array in a visible terminal window through a reusable, shell-free launch plan with dry-run, JSON, capability detection, detached fallback, and standalone recovery modes. Use when Codex needs to open an interactive CLI, SSH session, local development process, sandbox, or other argv-based command in a new host terminal; diagnose whether a supported terminal is available; or provide an actionable plan when the requested terminal is unsupported.
role: terminal-opener
category: engineering
triggers:
  - terminal opener
capabilities_required:
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/terminal-opener/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: terminal-opener
---

# terminal-opener

## Role

Portable distillation of upstream skill `terminal-opener` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Open an executable and its argument array in a visible terminal window through a reusable, shell-free launch plan with dry-run, JSON, capability detection, detached fallback, and standalone recovery modes. Use when Codex needs to open an interactive CLI, SSH session, local development process, sandbox, or other argv-based command in a new host terminal; diagnose whether a supported terminal is available; or provide an actionable plan when the requested terminal is unsupported.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
