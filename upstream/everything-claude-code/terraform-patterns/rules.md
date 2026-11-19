# Rules (extracted)

- Do not use workspaces as a substitute for separate production and non-production state with separate credentials.
- Never use `-lock=false` to get past a lock error. See [Debugging](#debugging).
- Do not configure `provider` blocks inside child modules. Declare `required_providers` and let the root pass providers in.
- Do not wrap a single resource in a module that only forwards its arguments.
