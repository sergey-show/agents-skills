# Destructive pattern table (portable)

| Pattern | Example | Risk |
|---------|---------|------|
| rm -rf / recursive deletes | `rm -rf /var/data` | Data loss |
| DROP TABLE/DATABASE | `DROP TABLE users` | Data loss |
| TRUNCATE | `TRUNCATE orders` | Data loss |
| git push --force | `git push -f origin main` | History rewrite |
| git reset --hard | `git reset --hard HEAD~3` | Work loss |
| git checkout/restore . | discards uncommitted | Work loss |
| kubectl delete | prod impact | Outage |
| docker rm -f / system prune | image/container loss | Recovery cost |
| Remove-Item -Recurse -Force | Windows wipe | Data loss |
| Format-Volume / Clear-Disk | disk wipe | Catastrophic |

Hard-deny candidates: recursive delete of `/` or home; force-push to main/master.
