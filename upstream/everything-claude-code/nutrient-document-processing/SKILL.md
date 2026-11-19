---
id: everything-claude-code__nutrient-document-processing
name: nutrient-document-processing
version: 1.0.0
description: >-
  Process, convert, OCR, extract, redact, sign, and fill documents using the Nutrient DWS API. Works with PDFs, DOCX, XLSX, PPTX, HTML, and images. Use when converting, OCRing, extracting from, redacting, signing, or filling documents via the Nutrient DWS API.
role: nutrient-document-processing
category: meta
triggers:
  - nutrient document processing
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/nutrient-document-processing/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: nutrient-document-processing
---

# nutrient-document-processing

## Role

Portable distillation of upstream skill `nutrient-document-processing` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Process, convert, OCR, extract, redact, sign, and fill documents using the Nutrient DWS API. Works with PDFs, DOCX, XLSX, PPTX, HTML, and images. Use when converting, OCRing, extracting from, redacting, signing, or filling documents via the Nutrient DWS API.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
