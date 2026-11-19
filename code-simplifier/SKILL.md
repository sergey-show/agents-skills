---
id: code-simplifier
name: Code Simplifier
version: 1.0.0
description: >-
  Reduces complexity without changing behavior: delete, reuse, merge,
  split-by-job, kill YAGNI abstractions. Use when code is over-engineered,
  after features land, or when asked to simplify.
role: Simplification Engineer
category: engineering
triggers:
  - simplify
  - deslop
  - reduce complexity
  - yagni cleanup
  - delete dead code
  - code simplification
capabilities_required:
  - filesystem.read
  - search.code
  - filesystem.edit
capabilities_optional:
  - test.run
  - git.ops
  - ask_user
sources:
  - research/agent-skills/skills/code-simplification
  - research/ponytail
harness: any
---

# Code Simplifier

## Role
Every extra line must be read, tested, and fixed later. Simplify behavior-preservingly: delete dead code, reuse existing helpers, prefer stdlib, collapse needless abstractions.

## When to use
Over-engineering complaints; post-feature cleanup; explicit simplify/deslop; review found lean issues.

## Workflow
1. Characterize behavior with tests or clear manual checks.
2. Apply simplify operators (delete/reuse/stdlib/yagni/merge/split).
3. Keep tests green; no behavior change unless user asked.
4. Report what was removed and residual risks.

## Done when
Diff smaller or clearer; behavior preserved (tests); no new abstractions for their own sake.

## See also
- Related: `minimal-coder`, `staff-reviewer`

## Upstream depth

- `skills/upstream/agent-skills/code-simplification/`
- `skills/upstream/ponytail/ponytail/`
- `skills/upstream/gstack/deslop-shared-libs/`
