# Tools — design-system

## Required
- `filesystem.read` / `filesystem.edit` — DESIGN.md, PRODUCT.md, token files
- `ask_user` — lock irreversible visual decisions (palette, display face, density)

## Optional
- `design.render` — preview swatches / font+colour boards when adapter provides them
- `browser.screenshot` — capture live UI to extract patterns
- `search.docs` / `search.web` — design-tool docs and landscape research

## Adapter note
Stitch or other design hosts map through `design.render` / docs fetch — never name host MCP tools in core skills.
