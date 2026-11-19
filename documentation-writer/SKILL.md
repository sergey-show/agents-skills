---
id: documentation-writer
name: Documentation Writer
version: 1.0.0
description: >-
  Writes and updates docs and ADRs: decision records, release notes, how-
  to guides. Use when documenting decisions, generating release
  documentation, or repairing stale docs.
role: Documentation / ADR Author
category: engineering
triggers:
  - write an ADR
  - architecture decision record
  - update the docs
  - release notes
  - document this
  - document-generate
capabilities_required:
  - filesystem.read
  - filesystem.edit
  - search.code
capabilities_optional:
  - git.ops
  - ask_user
  - search.docs
sources:
  - research/agent-skills/skills/documentation-and-adrs
  - research/gstack/document-generate
  - research/gstack/document-release
harness: any
---

# Documentation Writer

## Role
Durable documentation for humans and agents: ADRs for decisions, accurate how-tos, honest release notes. Docs match the code that exists — not aspirational systems.

## When to use
New architectural decisions; release documentation; onboarding docs; fixing stale README/sections; user asks to document.

## Workflow
1. Read code + existing docs; note drift.
2. Choose artifact: ADR vs how-to vs reference vs release notes.
3. Write with templates; link related ADRs.
4. Verify commands/paths against the repo.
5. Mark superseded ADRs — never silently rewrite history.

## Done when
Doc accurate to current code; ADR status clear; release notes only claim verified changes.

## See also
- [approaches.md](approaches.md)

## Upstream depth

- `skills/upstream/agent-skills/documentation-and-adrs/`
- `skills/upstream/gstack/document-generate/`
- `skills/upstream/gstack/document-release/`
