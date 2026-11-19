# Approaches — design-director

## 1. Pre-flight (before asking)

Signals in order:
1. Root `DESIGN.md` / `design.md` — locked system overrides free direction.
2. Brand spec or named real brand — never invent brand truth from memory.
3. Project fonts, palette, spacing, motion, framework (`package.json`, tokens, `:root`).
4. The product itself (URL, dev server, runnable app) — prefer real captures over drawn UI.
5. Existing PRODUCT.md users/jobs — grounds persona and hierarchy choices.

Emit one short preflight block: what is preserved vs introduced (file:line when useful).

## 2. Ask once

Four fields in one message: **Material** (real numbers, quotes, logos, photos, product screens), **Audience**, **Use** (one primary action), **Tone** (an extreme — not "clean and modern"). Skipped fields are opt-outs: infer, state the inference once, stamp it. Facts are never inferred.

Genre heuristic (silent): atmospheric / modern-minimal / playful / editorial. Scope: component vs app screen vs marketing page.

## 3. Shape → Direction

- **Material inventory:** real / pictures / absent (proof you will not invent).
- **Job + anatomy:** what a visitor came to do; build sections from category anatomy, not the default hero→3 features→email band.
- **Signature:** the one memorable real thing on the first screen.
- **Direction:** user-named theme, custom ask, or a dealt distinctive direction that clears recent builds (mirror test: would a neighbour prompt get the same combination? If yes, change one decision).

## 4. Craft floor (verify on the built result)

Batched checks — one render pass, not separate trips:
- Contrast ≥4.5:1 body / ≥3:1 large; tint secondary text from surface hue
- Depth: shadows with offset + blur (no zero-offset glow halo)
- Spacing: tight groups, generous separation; more space above a head than below
- Type: body ~65–75ch; balanced heads; no overflow at breakpoints
- Motion: one authored moment; transform/opacity; reduced-motion fallback; visible without JS
- States: hover, focus-visible, disabled, loading, error, empty
- Browser surfaces: selection, caret, scrollbar, focus rings themed
- Copy: product nouns; controls name actions; no invented metrics

## 5. Anti-slop / house bans (portable)

From Hallmark Floor + Impeccable refuse + Stitch taste-design + Taste house rules:
- No purple-to-blue / cyan-on-dark AI gradients; no cream+serif+terracotta cliché unless brand pins it
- No Inter/Roboto/Arial/Poppins as display when brand work allows choice
- No eyebrow / tracked-caps label stacks; no middle-dot meta strings; no "Learn more →"
- No nested cards; no three equal icon+heading cards as the page structure
- No emoji-as-icon; no hand-drawn browser/OS chrome; no fake product UI when the real product is reachable
- No invented metrics, testimonials, logo walls; no filler ("Scroll to explore")
- Hero: headline + one sentence + primary action visible at ~1280×800 without scroll
- One idea per screen; ~80 words per viewport; cards only when they contain interaction

## 6. Plan-design review (gstack portable)

When the target is a **plan**, not a live page:
1. Scope gate: confirm plan path / branch diff / pasted doc.
2. Audit missing design decisions (hierarchy, empty/error states, density, motion, responsive, brand).
3. **Add decisions into the plan** — output is a better plan, not a memo about the plan.
4. Optional mockups only after decisions are written.

## 7. Live design review / polish

Score dimensions 0–10 against a written "what 10 looks like": hierarchy, specificity, restraint, consistency, states, a11y. Fix FAIL/REFLEX before polish. Polish never smuggles a redesign — if the concept is wrong, say so and route to redesign.

## 8. Sweep & fresh-context review

1. Mechanical Floor checks (lint/detector/manual equivalent).
2. Walk Reflex gates: fix or waive with gate id + guard evidence + page-specific reason.
3. Answer Finish craft findings.
4. Prefer a fresh subagent for hero-then-finish review when `subagent.spawn` exists; otherwise re-read cold and mark `in-thread`.
5. Close with the material ask: what real asset would most improve the page.

## Sources of taste
- Hallmark: Floor/Reflex/Finish gates, deal diversity, hero-first build
- Impeccable: craft-floor, critique dual-assessment, polish triage
- Taste Skill: finish gate rounds, consistency + layout checks
- Stitch taste-design: dials + explicit bans list
- gstack: plan-design-review, design-review score loops
