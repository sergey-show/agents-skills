---
id: taste-skill__taste-skill
name: design-taste-frontend
version: 1.0.0
description: >-
  tasteskill 2.5.1, the anti-slop frontend skill. Builds professional company websites at the level of figma.com and x.ai: plain copy in a voice of its own, one system, one section per screen, equal edges, real photographs and real product UI (licensed stand-in photographs when the client has none; a product render only when the brief asks for 3D), a hero entrance and one or two dealt moments on every page, shader effects and scenes only on tech, gaming and software pages, quiet micro-interactions, and a checker and finish gate that enforce it in a real browser. Use this whenever you build, design, redesign, restyle, polish or review a landing page, company, product, shop, cafe, hotel, studio, SaaS, AI, developer-tool or game site, as static HTML/CSS or inside an existing React, Next.js, Vue, Svelte, Astro or Tailwind project, or when the user says a page looks generic, templated or "AI-made".
role: design-taste-frontend
category: design
triggers:
  - taste skill
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
sources:
  - research/taste-skill/skills/taste-skill/SKILL.md
harness: any
upstream_repo: taste-skill
upstream_skill: taste-skill
---

# design-taste-frontend

## Role

Portable distillation of upstream skill `taste-skill` from `taste-skill`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

tasteskill 2.5.1, the anti-slop frontend skill. Builds professional company websites at the level of figma.com and x.ai: plain copy in a voice of its own, one system, one section per screen, equal edges, real photographs and real product UI (licensed stand-in photographs when the client has none; a product render only when the brief asks for 3D), a hero entrance and one or two dealt moments on every page, shader effects and scenes only on tech, gaming and software pages, quiet micro-interactions, and a checker and finish gate that enforce it in a real browser. Use this whenever you build, design, redesign, restyle, polish or review a landing page, company, product, shop, cafe, hotel, studio, SaaS, AI, developer-tool or game site, as static HTML/CSS or inside an existing React, Next.js, Vue, Svelte, Astro or Tailwind project, or when the user says a page looks generic, templated or "AI-made".

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
