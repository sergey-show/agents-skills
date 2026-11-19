# Approaches — qa-lead

## Core loop: Explore → Reproduce → Regress → Fix → Re-verify

Keep a short evidence log:
- Environment (URL, build, account role)
- Steps
- Expected vs actual
- Artifact paths (snapshot, screenshot, HAR, log excerpt)

## Snapshot-before-act (Chrome DevTools portable)

1. Navigate (or confirm current page).
2. Wait on a real condition (text/role/network idle) — never flaky sleeps.
3. Take an accessibility snapshot / structured tree.
4. Interact using stable element refs/uids from that snapshot.
5. If the element is missing, re-snapshot — do not guess selectors from memory.

Order is mandatory: navigate → wait → snapshot → interact. Parallel calls must preserve that order.

## Efficient evidence

- Prefer a11y snapshots over full DOM dumps and over screenshots for structure.
- Use screenshots for visual/layout bugs only.
- Paginate/filter network and console output; write large artifacts to files and cite paths.
- Quote console/network errors — never invent them.

## gstack QA portable methodology

1. Charter: what "works" means for this session.
2. Happy path first; then edge, empty, error, permission, slow network.
3. File bugs with severity and repro; fix P0/P1 in-session when scope allows.
4. After fix: same steps, same environment, attach before/after.
5. Leave a regression the next agent can run.

## Non-web QA

Same loop for CLIs, APIs, workers, webhooks: invoke → assert → regress → fix → re-invoke. Capture command, status, stdout/stderr tails.

## Specialized handoffs

- Auth/cookie/session weirdness → `browser-debugger` cookie methodology
- A11y failures → `a11y-auditor`
- LCP / jank → `webperf-auditor`
- Suspected leaks → memory-leak methodology in `browser-debugger`

## Diagnose before edit

Inventory failures. Preserve the original failing test/signal. Do not "fix" by deleting assertions or skipping the path that caught the bug.
