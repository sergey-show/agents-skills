# Approaches — browser-debugger

## Core loop

```
navigate → wait(condition) → snapshot → interact → (network|console|cdp) → hypothesize → verify
```

Never invert: do not click before a fresh snapshot when the DOM just changed. Prefer condition waits (text/role/network) over sleeps.

## Snapshot-before-act

1. Confirm page / `page` target.
2. Wait until the UI under test is ready.
3. Take an accessibility / structured snapshot; note element refs/uids.
4. Interact with those refs only.
5. If missing → re-snapshot; do not invent selectors from memory.

Prefer a11y tree for structure; screenshots for paint/overlap; evaluate snippets for computed facts (contrast, sizes) sparingly.

## Efficient data

- Write large screenshots / snapshots / traces to files; cite paths.
- Paginate and filter network (`resourceTypes`, status).
- Filter console to `error` / `issue`; include preserved messages for load-time problems.
- Disable include-snapshot on noisy fill/click storms unless you need the update.

## Cookie / auth debugging (portable)

| Need | How |
|------|-----|
| Read HttpOnly | Request `Cookie` / response `Set-Cookie` via network — not `document.cookie` |
| Read non-HttpOnly | `cookieStore.getAll()` / document.cookie when available |
| Active 401/403 | Live tab; inspect failing request headers |
| Consent / first visit | **Isolated clean context**; close when done |
| Attributes | Domain, Path, Secure, SameSite, Expires/Max-Age mismatches |

Silent failure: JS cannot clear HttpOnly — use a clean context instead.

## CSS / runtime

Computed styles and cascade beat guessing. Prefer logpoints / breakpoints over editing production source for temporary probes when CDP allows.

## Memory-leak methodology (portable)

1. Baseline heap snapshot.
2. Repeat the suspect interaction ~10× to amplify growth.
3. Revert UI to start state; take final snapshot.
4. Compare **summaries** first; then class growth; then retainers / dominators / edges.
5. Useful filters: detached DOM, event handlers, contexts, console retention, duplicate strings.
6. Close loaded snapshots when finished (server memory).
7. Ask before nulling objects that may be intentional caches.

## Performance handoff

For LCP/CWV: record a reload performance trace, identify the LCP element, note insight names (breakdown, discovery, render-blocking), and hand the package to `webperf-auditor`.

## Extension / service worker

Only when the harness exposes those capabilities. If missing, document the prerequisite — do not fake results.

## Forensic note template

- Environment / URL / account
- Hypothesis
- Steps + evidence paths
- Root cause (or blocker)
- Suggested fix owner (`qa-lead` regression, app code, infra)
