# Approaches — performance-engineer

Distilled from agent-skills performance-optimization and chrome-devtools-mcp debug-optimize-lcp (capabilities abstracted).

## CWV targets
| Metric | Good | NI | Poor |
|--------|------|----|------|
| LCP | ≤2.5s | ≤4s | >4s |
| INP | ≤200ms | ≤500ms | >500ms |
| CLS | ≤0.1 | ≤0.25 | >0.25 |

## Workflow
MEASURE → IDENTIFY → FIX → VERIFY → GUARD. Use both synthetic (repro/CI) and RUM (real users) when possible.

## Symptom → where to measure
- First load → bundle, LCP element, TTFB, render-blocking
- Interaction lag → main-thread long tasks, INP
- API slow → server timing, DB explain, N+1
- Memory → heap growth, listener leaks

## LCP portable workflow
1. Load page; capture performance trace with reload.
2. Analyze LCP breakdown insights (subparts).
3. Identify LCP element (tag, resource URL, timings).
4. Inspect network waterfall for that resource (start delay vs duration).
5. Audit HTML issues: lazy-loading viewport LCP image, missing fetchpriority, render-blocking scripts.

### LCP subparts
| Subpart | Ideal share | Meaning |
|---------|-------------|---------|
| TTFB | ~40% | nav → first HTML byte |
| Resource load delay | <10% | TTFB → start LCP resource |
| Resource load duration | ~40% | download |
| Element render delay | <10% | downloaded → painted |

Optimize the actual bottleneck subpart — compressing an image won't help if render delay dominates.

### Common LCP fixes (by subpart)
- TTFB: caching, edge, faster origin, less server work
- Load delay: discover LCP in initial HTML; `fetchpriority=high`; don't lazyload hero
- Load duration: compress/resize/CDN; modern formats
- Render delay: reduce blocking CSS/JS; avoid late-discovered fonts that delay text LCP

## Backend / data
Kill N+1; add indexes from EXPLAIN; cache carefully with invalidation plan; avoid unbounded work on request path.

## Guard
Performance budgets in CI when project has them; document the metric you moved.
