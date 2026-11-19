# Approaches — a11y-engineer

Distilled from agent-skills accessibility-engineering and chrome a11y-debugging (portable).

## Phase routing
New component construction → `frontend-engineer`. This skill: audit/remediate existing UI.

## Automated audit
Run project or standard axe/pa11y-style checks against the running page. Keep JSON reports when useful. Severities: Critical / Serious / Moderate / Minor. **Verify each hit in the browser** — drop false positives.

## Manual — keyboard
Tab all interactives with visible focus; Enter/Space activate; Escape closes dialogs; arrows where expected; no keyboard traps.

## Manual — screen reader
Headings logical; landmarks labeled; links make sense out of context; form labels + errors announced; live updates announced.

## Manual — visual
Contrast 4.5:1 text / 3:1 large & UI; zoom 200% without overlap; forced colors; prefers-reduced-motion honored; focus ring visible on all backgrounds.

## Remediation order
Critical → Serious → Moderate → Minor. Prefer semantic HTML before ARIA. If using ARIA, follow rules of ARIA (don't override native semantics needlessly).

## Chrome a11y debugging (portable)
Use accessibility tree snapshots to see computed names/roles; confirm focus order matches visual order; check name computation for buttons/links/inputs.
