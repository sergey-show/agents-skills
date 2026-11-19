# agents-skills

Harness-agnostic agent skills — portable roles, tools, approaches, and rules for Cursor, Claude Code, Codex, OpenCode, Gemini, Copilot, or any agent that reads `SKILL.md`.

Skills use abstract capabilities (`filesystem.edit`, `ask_user`, `browser.navigate`, …), not vendor MCP names.

## Layout

| Path | Contents |
|------|----------|
| `_meta/` | Format + manifest |
| `_tools/` | Capability vocabulary |
| `<role>/` | Curated role (`SKILL.md`, `tools.md`, `approaches.md`, `rules.md`) |
| `upstream/` | Ports of upstream open-source skills |

## Install

Copy this repository (or selected role folders) into your agent's skills directory.

## License

MIT for this pack — see `LICENSE`. Upstream-derived ports: `THIRD_PARTY.md`.
