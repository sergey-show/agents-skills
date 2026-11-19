# Approaches — design-auditor

## Critique (Impeccable portable)

### Hard invariants
- Assessment A (design) and B (detector/browser) both required on web when tools exist.
- Prefer isolated subagents so detector output does not anchor design judgment early.
- Viewable targets need browser inspection when available.
- Report first; question last.
- Incomplete without closing questions or `Questions skipped: <reason>`.

### Assessment A — Design review
Evaluate: design specificity (could another product wear this UI unchanged?), hierarchy/IA, emotional fit, typography/color, states, copy, cognitive load, Nielsen heuristics (0–4 or n/a), persona red flags on the primary action. Return 2–3 strengths, 3–5 priority issues, provocative questions.

### Assessment B — Evidence
- Static/detector findings with file locations
- Browser: contrast, focus order via snapshot Tab walk, overflow at 390/1440, console a11y issues
- Note false positives; never claim overlay/injection succeeded unless it did

### Synthesis
Merge without double-counting. Separate judgment from measurement. Persist a snapshot summary if the project keeps critique history; otherwise deliver in-chat.

## Technical audit dimensions (score 0–4 each)

See [references/audit-dimensions.md](references/audit-dimensions.md): Accessibility · Performance · Theming · Responsive · Implementation Integrity. Total /20 with rating bands.

Severity tags: P0 blocking · P1 major/WCAG AA · P2 minor · P3 polish.

## Detect / polish input
A detector result is defect evidence, not proof of quality. Polish triage order: broken tasks → missing states → system drift → visual/motion → cleanup. Hand polish execution to `design-director` unless asked to fix here.

## Hallmark audit verb
When asked only for an audit report on an existing design: report Floor/Reflex/Finish findings; do not redesign unless named.
