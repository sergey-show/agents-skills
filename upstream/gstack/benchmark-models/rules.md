# Rules (extracted)

- Never print a whole environment, git config or process table; tokens ride in them. Banned: `env`, bare `printenv`, `set` or `export` (or an empty `export $(...)`), `export -p`/`-n`, `declare -p`/`-x`, `typeset -p`, `set -x`, `git config --list`/`-l`, any `ps` with full args (`aux`, `-ef`, `-o args`), `docker top ... args`, `docker inspect` Env. Read one value by name (`git config --get <name>`), check a variable with `[ -n "${NAME:-}" ] && echo set`, list processes by name or pid.
