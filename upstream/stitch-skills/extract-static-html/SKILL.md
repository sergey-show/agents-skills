---
id: stitch-skills__extract-static-html
name: stitch::extract-static-html
version: 1.0.0
description: >-
  Extract self-contained static HTML from a built web application or React components by inlining CSS and images. Use this skill whenever you need to capture a specific UI state, share a static version of a page, or prepare assets for Stitch upload, even if the user just asks to 'save the HTML' or 'mock the view'.
role: stitch::extract-static-html
category: design
triggers:
  - extract static html
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - subagent.spawn
sources:
  - research/stitch-skills/plugins/stitch-design/skills/extract-static-html/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: extract-static-html
---

# stitch::extract-static-html

## Role

Portable distillation of upstream skill `extract-static-html` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Extract self-contained static HTML from a built web application or React components by inlining CSS and images. Use this skill whenever you need to capture a specific UI state, share a static version of a page, or prepare assets for Stitch upload, even if the user just asks to 'save the HTML' or 'mock the view'.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
