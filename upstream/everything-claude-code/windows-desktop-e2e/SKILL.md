---
id: everything-claude-code__windows-desktop-e2e
name: windows-desktop-e2e
version: 1.0.0
description: >-
  E2E testing for Windows native desktop apps (WPF, WinForms, Win32/MFC, Qt) using pywinauto and Windows UI Automation. Use when writing E2E tests for a Windows native desktop app with pywinauto or UI Automation.
role: windows-desktop-e2e
category: design
triggers:
  - windows desktop e2e
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/windows-desktop-e2e/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: windows-desktop-e2e
---

# windows-desktop-e2e

## Role

Portable distillation of upstream skill `windows-desktop-e2e` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

E2E testing for Windows native desktop apps (WPF, WinForms, Win32/MFC, Qt) using pywinauto and Windows UI Automation. Use when writing E2E tests for a Windows native desktop app with pywinauto or UI Automation.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
