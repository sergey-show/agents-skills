---
id: agent-skills__debugging-and-error-recovery
name: debugging-and-error-recovery
version: 1.0.0
description: >-
  Guides systematic root-cause debugging. Use when tests fail, builds break, something that worked yesterday broke, behavior doesn't match expectations, or you encounter any unexpected error. Use when you need to figure out what broke and why — a systematic approach to finding and fixing the root cause rather than guessing. Use when asked what broke, why a test started failing, or why code throws, even when the diff, the function, or the stack trace is pasted inline and the cause looks obvious from reading it, so that the cause is named, the fix is minimal, and the reply says how to confirm it.
role: debugging-and-error-recovery
category: engineering
triggers:
  - debugging and error recovery
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/debugging-and-error-recovery/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: debugging-and-error-recovery
---

# debugging-and-error-recovery

## Role

Portable distillation of upstream skill `debugging-and-error-recovery` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Guides systematic root-cause debugging. Use when tests fail, builds break, something that worked yesterday broke, behavior doesn't match expectations, or you encounter any unexpected error. Use when you need to figure out what broke and why — a systematic approach to finding and fixing the root cause rather than guessing. Use when asked what broke, why a test started failing, or why code throws, even when the diff, the function, or the stack trace is pasted inline and the cause looks obvious from reading it, so that the cause is named, the fix is minimal, and the reply says how to confirm it.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
