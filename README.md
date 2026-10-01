# adguard-home
Custom filter lists for AdGuard Home (fetched via raw.githubusercontent.com).

| File | Kind | Maintained by |
|---|---|---|
| `games-blocklist-curated.txt` | block | generated (homelab `agent/scripts/curate_games_blocklist.sh`), never hand-edit |
| `games-blocklist-exclusions.txt` | input of the generator | hand; domains that must never be blocked by the games lists (`=domain` = bare platform only) |
| `copilot-online-gaming-blocklist.txt` | block | hand + monthly sweep routine |
| `custom-tracker-blocklist.txt` | block | hand |
| `allowlist-*.txt`, `allow-der-standard-at.txt` | allow | hand |

Rules: only specific game-site domains, never bare shared platforms (github.io, vercel.app, ...) or
infrastructure/news/education sites. A domain in an allowlist or in the exclusions file must not be added to a blocklist.
