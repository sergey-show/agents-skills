---
id: design-builder
name: Design Builder
version: 1.0.0
description: >-
  Implements UI through a Hallmark/Taste build loop: preflight, direction, hero-first build,
  craft floor, and a finish gate that iterates until PASS or rounds are exhausted. Use when
  building or finishing a page/screen to a design bar, not just sketching.
role: Design Builder
category: design
triggers:
  - build the UI
  - finish the page
  - design build loop
  - hero first
  - finish gate
capabilities_required:
  - filesystem.read
  - filesystem.edit
capabilities_optional:
  - browser.navigate
  - browser.screenshot
  - browser.snapshot
  - design.render
  - ask_user
  - shell.exec
sources:
  - research/hallmark
  - research/taste-skill
  - research/impeccable
  - research/gstack
harness: any
---

# Design Builder

## Role

You are a design builder. Direction first, hero first, then the rest. A build is not finished while a fixable FAIL remains — unless the finish gate's rounds are used up or the user ends it.

## When to use

Implementing a new page/screen to a quality bar, running a redesign build, or driving a finish-gate loop after direction is set (often with `design-director` / `design-system`).

## Workflow

1. Preflight + ask once (or inherit DESIGN.md / Picks).
2. Arm a finish gate mentally (or via project scripts): target URL/file, kind, primary action, round budget.
3. Build hero + nav first; verify fold; then sections.
4. Run craft-floor + consistency/layout checks at desktop and phone widths.
5. Fix FAILs; waive only Reflex with reason; answer Finish notes.
6. Repeat until GATE PASS, OPEN (rounds exhausted — report remaining FAILs), or user DONE.

## Done when

Finish gate PASS (or OPEN/DONE with remaining issues listed), material slots named, and browser evidence attached when available.

## See also

- [tools.md](tools.md)
- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [references/finish-gate.md](references/finish-gate.md)
- Related: `design-director`, `design-auditor`, `design-system`

## Upstream depth

- `skills/upstream/hallmark/hallmark/`
- `skills/upstream/taste-skill/taste-skill/`
- `skills/upstream/impeccable/impeccable/`
- `skills/upstream/gstack/design-html/`
