# Approaches — frontend-engineer

Distilled from agent-skills frontend-ui-engineering and ECC frontend-patterns (portable).

## Verify with what the project has
Run project test/typecheck/lint. Don't install frameworks just to verify. If none, review against checklist and say what you couldn't run.

## Architecture
Colocate component, test, stories, hooks, types. Composition over mega-props configuration. Focused components; compound components for related UI state (tabs, etc.).

## State
Local state first; lift only when needed. Server state libraries when project already uses them. Avoid duplicating server state in ad-hoc globals.

## Accessibility while building
Semantic elements; label inputs; manage focus on dialogs/routes; don't rely on color alone; hit targets; respect reduced motion.

## Styling
Use the project's design tokens/system. No one-off magic numbers that fight the system. Responsive: mobile constraints first when project does.

## Performance habits
Avoid needless re-renders; virtualize large lists when needed; code-split routes; don't lazyload above-the-fold LCP content.

## Anti-AI-slop (engineering lens)
No generic purple gradients / interchangeable card grids unless the design system says so. Follow `design-director` / `design-system` when brand is in scope.

## Patterns (ECC portable)
Composition; controlled vs uncontrolled inputs clearly; error boundaries at route level when applicable; data fetching consistent with repo (Suspense/query lib/etc.).
