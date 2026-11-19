---
id: gstack__make-pdf
name: make-pdf
version: 1.0.0
description: >-
  Turn any markdown file into a publication-quality PDF. Use for: markdown to pdf, generate pdf, make pdf, export pdf. (gstack)
role: make-pdf
category: meta
triggers:
  - make pdf
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
  - research/gstack/make-pdf/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: make-pdf
---

# make-pdf

## Role

Portable distillation of upstream skill `make-pdf` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Turn any markdown file into a publication-quality PDF. Use for: markdown to pdf, generate pdf, make pdf, export pdf. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
