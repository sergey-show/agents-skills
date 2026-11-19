# Approaches — a11y-auditor

## Modes (agent-skills portable)

- **Deep:** axe-core / pa11y / Lighthouse a11y JSON and/or live browser accessibility tree + keyboard walk.
- **Quick:** source anti-patterns only (div-as-button, missing labels/alt, skipped headings, no focus styles, click handlers without keyboard). Label the report incomplete for AA claims.

If Deep was intended but artifacts/browser caps are missing, say what is blocked.

## Live debugging (Chrome DevTools portable)

1. **Automated baseline** — Lighthouse a11y (navigation mode) or axe JSON. Filter failures only (`score < 1`); never paste the whole report into chat.
2. **Browser issues** — console/issue channel for missing names, invalid ARIA, contrast warnings preserved across load.
3. **Semantics & structure** — accessibility snapshot: heading levels (no skips), landmarks, lists, tables with headers.
4. **Reading order** — screenshot vs tree order; flag CSS that visually reorders content away from DOM/AT order.
5. **Names & forms** — every control has an accessible name; associate `<label>` / `aria-labelledby`; find orphaned inputs; images need alt or `aria-hidden` if decorative.
6. **Keyboard** — Tab / Shift+Tab walk with re-snapshot after each move; confirm focus target; modals move focus in and trap until dismissed; Escape closes where expected; no unexpected focus loss.
7. **Focus visibility** — `:focus-visible` ring ≥3:1 against adjacent background; never remove outline without a replacement.
8. **Tap targets** — ~48×48 CSS px guidance (WCAG 2.5.8 allows 24×24 with spacing exceptions); measure via evaluate when available.
9. **Contrast** — body ≥4.5:1, large text ≥3:1; tint secondary text on coloured surfaces; verify dark theme pairs.
10. **Document & motion** — `lang`, `<title>`, skip link, `prefers-reduced-motion` alternatives that preserve state change (not a global 0.01ms kill that erases feedback).

## Source Quick scan tells

| Tell | Why it fails users |
|------|--------------------|
| `<div onClick>` / roleless clickable | No keyboard / wrong role |
| `<img>` without alt | SR gap |
| Icon button with empty name | "Button" with no purpose |
| Heading level jumps | Lost outline |
| `outline: none` alone | Invisible focus |
| Colour-only error state | Fails non-visual / colour-blind |
| `aria-hidden` on focusable | Focus black hole |
| Positive `tabIndex` soup | Broken order |

## Scoring & report

Map to **WCAG 2.2 AA**. Severity: **P0** blocks task · **P1** AA violation · **P2** annoying · **P3** polish. Note AAA approaches when relevant.

Report shape:
1. Mode + what was checked / skipped
2. Scorecard (sourced) or "unscored — Quick"
3. Ranked findings: location/selector · WCAG · impact · fix
4. Positive observations
5. Suggested next commands (`design-builder` for focus/tokens, `qa-lead` for regression)

## Design / ship overlap

Contrast, focus-visible, and reduced-motion also appear in design Floor gates and `design-auditor`. Cite once in `ship-gate` merges — keep the highest severity, don't triple-count.
