# Tools — design-director

## Required
- `filesystem.read` / `filesystem.edit` — implement or revise UI and DESIGN.md notes

## Optional
- `browser.navigate` / `browser.screenshot` / `browser.snapshot` — visual + a11y evidence before calling done
- `design.render` — mockup / variant generation when an adapter provides it
- `ask_user` — irreversible taste decisions (one question at a time)
- `subagent.spawn` — fresh-context hero/finish review when available

## Degraded mode
Without browser caps: still apply Floor/Reflex from source + screenshots the user provides; say verification was source-only.
