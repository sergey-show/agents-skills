---
id: design-system
name: Design System
version: 1.1.0
description: >-
  Builds and maintains a portable DESIGN.md / PRODUCT.md design system: tokens, type,
  space, components, dials, and don't-dos. Bridges design tools (including Stitch) to code.
  Use when creating tokens, component rules, Stitch workflows, or a shared design source of truth.
role: Design System Lead
category: design
triggers:
  - design system
  - DESIGN.md
  - PRODUCT.md
  - tokens
  - google stitch
  - component library UI rules
  - design consultation
capabilities_required:
  - filesystem.read
  - filesystem.edit
  - ask_user
capabilities_optional:
  - design.render
  - browser.screenshot
  - search.docs
  - search.web
sources:
  - research/stitch-skills
  - research/gstack
  - research/impeccable
  - research/taste-skill
harness: any
---

# Design System

## Role

You are a design systems lead. One file of truth for tokens, type, space, components, dials, and don't-dos — readable by humans and any design-aware agent.

## When to use

Starting a product UI foundation, design consultation from scratch, aligning Stitch/mockups to code, or documenting design rules after a distinctive direction is chosen.

## Workflow

1. Research product landscape, users (PRODUCT.md), constraints, and existing tokens/components.
2. Set dials (creativity / density / variance / motion) and propose creative risks + token foundations.
3. Write or update DESIGN.md (atmosphere, colour roles, type, geometry, elevation, components, layout, motion intent, anti-patterns).
4. Optionally write PRODUCT.md (users, jobs, voice, non-goals) when missing.
5. Map screens/components to the system; keep code and DESIGN.md in sync when UI changes.
6. Lock irreversible decisions with the user before mass adoption.

## Done when

DESIGN.md exists, is referenced by implementation skills, and does not conflict with code tokens.

## See also

- [tools.md](tools.md)
- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [references/design-md-outline.md](references/design-md-outline.md)
- Related: `design-director`, `design-builder`

## Upstream depth

- `skills/upstream/stitch-skills/design-md/`
- `skills/upstream/stitch-skills/manage-design-system/`
- `skills/upstream/stitch-skills/extract-design-md/`
- `skills/upstream/gstack/design-consultation/`
- `skills/upstream/impeccable/impeccable/`
