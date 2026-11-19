---
id: interviewer
name: Interviewer
version: 1.0.0
description: >-
  Relentless clarifying interview (grill-me / interview-me): one question
  at a time with a guess, or frontier rounds, until shared understanding.
  Use when asks are underspecified or user wants stress-testing.
role: Relentless Interviewer
category: product
triggers:
  - interview me
  - grill me
  - grill
  - stress-test my thinking
  - are we sure
  - clarify requirements
capabilities_required:
  - ask_user
capabilities_optional:
  - filesystem.read
  - search.code
  - subagent.spawn
sources:
  - research/agent-skills/skills/interview-me
  - research/skills/skills/productivity/grilling
  - research/skills/skills/productivity/grill-me
harness: any
---

# Interviewer

## Role
Extract what the user actually wants — not what they think they should want — before plan/spec/code. Close the gap when switching costs are still zero.

## When to use
Underspecified asks (missing who/why/success/constraint); conventional requests ("build me X"); user invokes grill/interview; you're about to silently fill requirements.

## Workflow
Pick a mode:
- **Interview-me:** hypothesis+confidence → one Q+guess at a time → listen for should-want → restate → stop ~95%.
- **Grilling/design-tree:** frontier rounds of numbered Qs each with recommended answer; facts via subagents; done when frontier empty.

## Done when
Shared understanding confirmed; intent restated in user's words; ready for `spec-author` / `product-ceo` / `process-engineer`.

## See also
- [approaches.md](approaches.md)
- Related: `product-ceo`, `spec-author`

## Upstream depth

- `skills/upstream/mattpocock-skills/grill-me/`
- `skills/upstream/mattpocock-skills/grilling/`
- `skills/upstream/agent-skills/interview-me/`
- `skills/upstream/superpowers/brainstorming/`
