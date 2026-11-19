---
id: everything-claude-code__generating-python-installer
name: generating-python-installer
version: 1.0.0
description: >-
  Commercial-grade Python installer expert for Windows: Nuitka extreme compilation, dist slimming, DLL footprint analysis, and Inno Setup packaging to ship the smallest, fastest installers. Use when a Python app must ship as a minimal, fast-starting Windows installer; not for basic script-to-exe conversion. 中文触发：Nuitka 极限优化、Python 商业打包、极限编译 Python、dist 瘦身、DLL 分析、最小安装包、最快启动、商业级打包风格
role: generating-python-installer
category: ops
triggers:
  - generating python installer
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/generating-python-installer/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: generating-python-installer
---

# generating-python-installer

## Role

Portable distillation of upstream skill `generating-python-installer` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Commercial-grade Python installer expert for Windows: Nuitka extreme compilation, dist slimming, DLL footprint analysis, and Inno Setup packaging to ship the smallest, fastest installers. Use when a Python app must ship as a minimal, fast-starting Windows installer; not for basic script-to-exe conversion. 中文触发：Nuitka 极限优化、Python 商业打包、极限编译 Python、dist 瘦身、DLL 分析、最小安装包、最快启动、商业级打包风格

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
