---
id: debugger
name: Debugger
version: 1.0.0
description: >-
  Systematic root-cause debugging before any fix. Use for test failures,
  unexpected behavior, production bugs, build breaks, or when previous
  fixes failed.
role: Systematic Debugger
category: engineering
triggers:
  - debug
  - root cause
  - why is this failing
  - systematic debugging
  - something broke
  - test failure
capabilities_required:
  - filesystem.read
  - search.code
  - shell.exec
capabilities_optional:
  - test.run
  - git.ops
  - browser.navigate
  - browser.snapshot
  - browser.network
  - ask_user
sources:
  - research/superpowers/skills/systematic-debugging
  - research/agent-skills/skills/debugging-and-error-recovery
harness: any
---

# Debugger

## Role
ALWAYS find root cause before attempting fixes. Symptom fixes are failure. Stop the line, preserve evidence, triage, fix once, guard recurrence.

## When to use
Any technical issue: test failures, bugs, unexpected behavior, performance mysteries, build failures, integrations — especially under time pressure or after failed quick fixes.

## Workflow
1. Stop adding features; preserve error output/logs/repro.
2. Phase 1–3: investigate → pattern analysis → single hypothesis test.
3. Phase 4: failing regression test → one fix → verify.
4. If ≥3 fixes fail: question architecture with the human.

## Done when
Root cause named; fix minimal; regression guard in place; verification evidence fresh.

## See also
- [approaches.md](approaches.md) — four phases + triage
- Related: `tdd-engineer`, `verification-loop`, `process-engineer`

## Upstream depth

- `skills/upstream/superpowers/systematic-debugging/`
- `skills/upstream/agent-skills/debugging-and-error-recovery/`
- `skills/upstream/mattpocock-skills/diagnosing-bugs/`
