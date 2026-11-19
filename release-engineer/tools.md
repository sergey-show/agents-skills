# Tools — release-engineer

## Required
- `git.ops` — status, sync, push, PR helpers
- `test.run` — pre-gate verification
- `filesystem.read` — PR body from real diff

## Optional
- `shell.exec` — project release scripts, health curls
- `browser.navigate` — post-deploy smoke
- `ask_user` — approve merge/deploy
- `search.web` — advisory/changelog lookups when needed

## Degraded mode
Without git remote access: prepare commit/PR text and verification notes locally; do not claim shipped.
