# DevTools playbook (capability map)

| Need | Capability | Notes |
|------|------------|-------|
| Structure / refs | browser.snapshot | a11y tree |
| Click/type | browser.interact | uid from snapshot |
| Visual | browser.screenshot | filePath for large |
| 401/Cookie | browser.network | Cookie / Set-Cookie |
| Console issues | browser.cdp or console list | types=issue/error |
| LCP | browser.cdp performance | reload trace |
| Leak | browser.cdp heap | compare summaries |
