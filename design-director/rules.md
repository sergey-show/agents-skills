# Rules — design-director

1. Do not ship a first viewport that could belong to any brand after removing the nav.
2. Do not default to dark-mode purple glow, purple-on-white gradients, or cream+serif+terracotta.
3. Do not add decorative components that do not serve the section's one job.
4. Preserve an existing design system when working inside one; encode new bans in DESIGN.md.
5. Prefer fewer elements with stronger hierarchy over more sections.
6. **Floor (never waive):** inventing metrics/quotes/logos; eyebrow + tracked-caps label stacks; nested cards; `transition: all` / animating layout geometry; skipping `:focus-visible` or `prefers-reduced-motion`; content hidden at rest without JS; emoji-as-icon; fake send/success states; pure `#000`/`#fff` outside tokens when a token system exists; horizontal overflow / `100vw` traps.
7. **Reflex (waive only with named gate + reason):** Inter/Roboto/system as display; three equal icon cards; gradient text; glow/wash blobs; cream-serif-terracotta; phone/laptop frames without real content; stock AI nav/footer; mono-as-costume.
8. Verify in a real browser (or screenshots at 375 / 768 / 1440) before calling UI done — LLM self-grade is not enough.
9. Prefer `DESIGN.md` / `PRODUCT.md` as durable context so later sessions converge less.
10. Never invent material. Absent proof stays absent (slots/placeholders), never fabricated.
11. For plan reviews: improve the plan itself; do not stop at advisory prose.
12. Fresh-context review when available; mark degraded if single-context.
