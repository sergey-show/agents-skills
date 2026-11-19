# Rules — browser-debugger

1. Snapshot before act; no flaky sleeps as the primary wait strategy.
2. Do not dump entire heaps/HARs into chat — summarize and cite files.
3. Do not treat JS cookie APIs as authoritative for HttpOnly.
4. Isolated context for consent/clean tests; don't contaminate with ambient auth.
5. Ask before destructive session clears on shared profiles.
6. Close large heap snapshots after investigation.
7. Declare missing optional caps instead of faking CDP results.
8. Quote errors; never invent console lines.
9. Prefer one-variable experiments.
10. Hand specialized a11y/LCP conclusions to the matching auditor skills when the deliverable is an audit report.
