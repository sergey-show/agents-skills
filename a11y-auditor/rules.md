# Rules — a11y-auditor

1. Prefer the accessibility tree over screenshots for semantics.
2. Do not claim WCAG AA compliance from Quick mode alone.
3. Filter automated reports — don't paste entire JSON into chat.
4. Every finding needs location/selector + WCAG ref when applicable + remediation.
5. Keyboard evidence requires an actual Tab walk when browser caps exist.
6. Opacity-hidden ≠ removed from the a11y tree — call out false "hidden".
7. Don't "fix" a11y by deleting features or `aria-hiding` real content.
8. Declare Deep vs Quick mode in the report header.
9. Never invent axe/Lighthouse failures — quote ids and selectors from artifacts.
10. Modal focus traps are intentional; page-wide traps are defects.
11. Colour must not be the sole state indicator.
12. Hand implementation fixes to builders only when asked; default deliverable is the audit.
