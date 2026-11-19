# Gate tiers (portable)

Distilled from Hallmark `gates.md` + Impeccable craft-floor. Harness-agnostic: enforce manually, via lint, or via detector adapters.

## How a gate binds

| Tier | Binding |
|------|---------|
| **Floor** | Never waivable. Correctness, access, honesty, and house rules that always read as machine-made. |
| **Reflex** | Model default. Waive only on the record with gate id, guard evidence, and a page-specific reason (<3 casual waivers; more → house style → DESIGN.md). |
| **Finish** | Craft detail. Reported and answered; never blocks ship alone. |
| **Ledger** | Repetition bookkeeping. Notes only. |

Grades: `FAIL` (Floor) · `REFLEX` · `WAIVED` · `WARN` · `ANSWERED` · `NOTE`. Nothing ships with open FAIL or unanswered REFLEX.

## Floor (must fix)

- Colour: purple-to-blue / purple-to-pink / cyan-on-dark AI gradients; colours/fonts as literals outside the token block when tokens exist
- Type: italic fragment inside a roman heading; tracked-caps / small-caps labels (house rule); uppercase display that can wrap with line-height < 1.0
- Structure: card-inside-card; hero sized in raw `vh` (use `dvh`/`svh`); horizontal scroll / missing overflow-x clip / `100vw`; image grid tracks on bare `1fr`; hero headline+lede+CTA not visible at 1280×800; container uncapped at 1920; ~80-word screen budget / hero with >2 text blocks before actions
- Chrome/copy: invented metrics/testimonials/logo walls; hand-drawn browser/OS chrome; eyebrows; template punctuation (· joined meta, arrows glued to links); fake form success
- Motion/a11y: `transition: all`; animating width/height/top/left; focus ring that fades in; missing `:focus-visible` (≥3:1); missing reduced-motion fallback; content hidden at rest requiring JS; emoji-as-icon; decorative SVG without aria-hidden/label; contrast failures; button labels that wrap

## Reflex (fix or waive with reason)

- Inter/Roboto/Open Sans/Poppins/Lato/system as display
- Gradient text (non-single-hue); glow/aurora/mesh blobs; cream paper + high-contrast serif + terracotta cliché
- Three equal icon-above-heading cards; AI template section run; identical section separators
- Mono as costume; bounce easing on UI; hover lift on every card; phone/laptop frames without real content; stock AI nav/footer
- Drawn illustration standing in for photos; empty gradient picture slots; counting-tick devices; photo-wall overload; fake product when real product is reachable; stock email-band close

## Finish (answer, don't block)

Straight quotes · ellipsis character · text-wrap balance on display · one primary button recipe · no icon-in-coloured-coin habit · tabular nums on figures · themed `::selection`/caret/scrollbar · heading levels not skipped · `lang` + title + meta description · no orphan words on heads

## Waiver form (stamp or DESIGN.md note)

```
waive <gate-id> · <guard evidence> · <why this page>
answered <finish-id> · <reason>
```

## Pre-emit critique axes (1–5)

Philosophy · Hierarchy · Execution · Specificity · Restraint · Variety. Anything under 3 revises before build. Name the weakest axis and the fix taken.
