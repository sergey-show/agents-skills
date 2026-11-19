# Tools — design-builder

## Required
- `filesystem.read` / `filesystem.edit` — implement UI, tokens, stamps

## Optional
- `browser.navigate` / `browser.screenshot` / `browser.snapshot` — gate evidence
- `design.render` — comps when available
- `ask_user` — material/direction locks; user DONE to close early
- `shell.exec` — project gate/lint scripts when present

## Degraded mode
Without browser: run source-level Floor checks and ask the user for screenshots; mark gate as source-only.
