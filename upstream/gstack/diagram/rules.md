# Rules (extracted)

- Never print a whole environment, git config or process table; tokens ride in them. Banned: `env`, bare `printenv`, `set` or `export` (or an empty `export $(...)`), `export -p`/`-n`, `declare -p`/`-x`, `typeset -p`, `set -x`, `git config --list`/`-l`, any `ps` with full args (`aux`, `-ef`, `-o args`), `docker top ... args`, `docker inspect` Env. Read one value by name (`git config --get <name>`), check a variable with `[ -n "${NAME:-}" ] && echo set`, list processes by name or pid.
- **Never ship the triplet without rendering it.** A `.mmd` file alone is not
  a diagram. If rendering is impossible (bundle missing, no browser available),
  say so and stop.
- For diagrams destined for a PDF: remind the user that `make-pdf` renders
  ` ```mermaid ` fences natively — embedding the `.mmd` in their markdown is
  better than embedding the PNG.
