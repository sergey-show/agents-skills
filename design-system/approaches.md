# Approaches — design-system

## 1. Design consultation loop (gstack portable)

1. Understand product: who, job-to-be-done, competitors, constraints.
2. Research landscape (visual references, not copy-paste).
3. Propose a complete system: aesthetic thesis, typography, colour roles, layout, spacing scale, motion principles.
4. Show a font+colour preview before locking.
5. Write DESIGN.md; optionally PRODUCT.md.
6. Hand off to `design-builder` / `design-director` for implementation.

## 2. Dials (Stitch taste-design portable)

Set before generating UI. Default bold-but-controlled: Creativity 7–9, Density 4–6, Variance 6–8, Motion 4–6.

| Dial | Low | High |
|------|-----|------|
| Creativity | Swiss, silent, mono | Editorial, asymmetric, inline imagery |
| Density | Gallery-airy | Cockpit-dense |
| Variance | Symmetric grids | No two sections alike |
| Motion Intent | Static | Orchestrated moments |

Record dial values in DESIGN.md so later agents inherit them.

## 3. DESIGN.md synthesis

From live screens, HTML export, or code:
1. Atmosphere in evocative adjectives (not "modern clean").
2. Colour palette: descriptive name + hex + functional role; pick ONE accent per project.
3. Typography: families, weight roles, tracking character, scale.
4. Geometry: radii described physically (pill / subtle / sharp).
5. Elevation: shadow quality (whisper / offset / flat).
6. Components: buttons, cards, inputs, nav, loaders, empty/error — with when-not-to-use.
7. Layout principles + responsive collapse rules.
8. Motion intent (code-phase notes even if mockups are static).
9. Explicit anti-patterns / bans.

Language: descriptive design terms + exact hex. Explain why, not only what.

## 4. PRODUCT.md (Impeccable portable)

Durable product context for design-aware agents:
- Product one-liner and non-goals
- Users / personas and primary jobs
- Voice and content rules
- Platforms and quality bar
- Links to DESIGN.md

## 5. Extract from code → system

When recovering a system from an existing app:
1. Inventory CSS variables / Tailwind theme / shared components.
2. Cluster colours into roles; kill one-off hexes into tokens or document exceptions.
3. Name the display/body/mono slots actually in use.
4. Capture real spacing scale from repeated values.
5. Write DESIGN.md that matches reality first, then propose cleanup diffs.

## 6. Stitch / design-tool bridge (capability level)

1. Retrieve screen metadata + HTML/CSS export via adapter.
2. Synthesize DESIGN.md from visual + code.
3. Use DESIGN.md as the prompt source of truth for new screens so agents converge.
4. When code drifts, update DESIGN.md in the same change or file a sync debt.

## 7. Token foundations

- Every token has a purpose statement.
- Semantic tokens (text/bg/border/accent/danger) over raw ramps in components.
- Dark mode: paired ink on every accent surface; never grey text on coloured panels.
- Space scale: one ladder; optical nudges are rare and named.
