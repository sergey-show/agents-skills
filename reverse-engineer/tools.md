# Tools — reverse-engineer

## Required
- `ask_user` — authorization, scope, and risk gates
- `filesystem.write` — evidence log + behavior spec

## Optional
- `reverse.inspect` — binary/package/firmware/managed analysis engines when available
- `browser.navigate` / `browser.network` / `browser.interact` — live web/Electron observation
- `shell.exec` — CLI fallbacks for JS/ASAR trees when engines exist
- `search.web` / `filesystem.read` — correlate with public docs

## Target routing (capability-level)
| Target | Approach |
|--------|----------|
| ASAR / Electron JS tree | Inventory → selected source analysis |
| ZIP/APK/IPA/MSIX/PyInstaller | Open archive → summary inventory → focused members |
| Managed PE/CLI | Managed inspect |
| Native binary | Static facts then optional runtime observation |
| Firmware | Region inspect / extract to new output dir only |
| Live browser / SPA | Capture with declared origins; export evidence bundles for long runs |
| Packet/signal recordings | Field discovery then decode with explicit filters |

## Levels
- **lite** — external behavior + network/file observation only
- **full** (default) — + artifact inspect when available
- **ultra** — + AgentEnv / scenario capture for replayable environments
