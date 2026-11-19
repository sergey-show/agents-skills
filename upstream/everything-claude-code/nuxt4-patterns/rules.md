# Rules (extracted)

- Do not use `route.fullPath` to drive SSR-rendered markup. URL fragments are client-only, which can create hydration mismatches.
