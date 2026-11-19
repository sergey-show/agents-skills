# Approaches — webperf-auditor

## Scope

Browser-facing web apps only. Refuse CLIs, pure libraries, and server-only services (point them at general performance engineering).

## Modes (agent-skills portable)

| Mode | Inputs | Finding label |
|------|--------|---------------|
| **Deep** | Lighthouse JSON, PSI, CrUX, DevTools trace, or live URL + browser caps | Measured |
| **Quick** | Source / bundle anti-patterns only | `potential impact` |

Declare the mode in the report header. If Deep was expected but inputs missing, say what to collect.

## LCP thresholds

- **Good** ≤ 2.5s
- **Needs improvement** 2.5–4.0s
- **Poor** > 4.0s

On most mobile pages the LCP element is an image — treat hero media as prime suspect.

## Four subparts (ideal share)

| Subpart | Ideal | Hunt when large |
|---------|-------|-----------------|
| TTFB | ~40% | slow origin, redirects, uncached HTML |
| Resource load delay | <10% | late discovery, `loading="lazy"` on LCP, CSS `background-image`, JS-injected src |
| Resource load duration | ~40% | weight, format, no CDN, no cache |
| Element render delay | <10% | blocking CSS/JS, long tasks, client-only render |

**Common pitfall:** compressing an image when render delay is the bottleneck — saved bytes shift into delay, LCP barely moves.

## Deep workflow

1. Navigate to the URL; start a performance trace **with reload**.
2. Analyze insights: LCP breakdown, document latency, render-blocking, LCP discovery.
3. Identify the LCP element (tag, resource URL, timings). Empty URL ⇒ text LCP.
4. Network waterfall for that resource: start time vs first byte/first resource; download duration.
5. HTML/common-issue audit: lazy LCP, missing `fetchpriority="high"`, missing preload, sync scripts in head.
6. Prescribe fixes **by bottleneck subpart** (see [references/lcp.md](references/lcp.md)).
7. Re-trace to verify; optionally emulate Slow/Fast 3G and 4× CPU — label lab ≠ field when CrUX absent.

## Quick source tells

- Hero `<img loading="lazy">` or CSS-only hero image
- Multi‑MB PNG/JPEG without modern formats / `srcset`
- Sync third-party scripts in `<head>`
- Animating layout properties / unbounded filters
- Fonts blocking without `font-display: swap|optional`
- Huge unsplit client bundles on landing routes
- Missing CDN / cache headers on static media (when config is in-repo)

## Other CWV (brief)

When asked beyond LCP: note CLS (reserve space, no late font swap jumps) and INP (long tasks, heavy handlers). Still lead with measured evidence.

## Report

1. Mode + artifact provenance
2. Scorecard with **sourced** numbers only (blank if unknown)
3. Ranked findings: subpart · evidence · fix · expected effect
4. Positives / already-good patterns
5. Verification plan (second trace, field CrUX)
