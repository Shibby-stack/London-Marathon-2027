# Lessons

- Keep the raw Strava export out of git: it contains email, contacts and followers. Commit only the cleaned run table.
- Artifact pages rely on the platform's `[hidden]{display:none}` rule. Any element given its own `display` must also have a `[hidden]` rule, or it covers the page when tested outside the artifact viewer.
- Claude's GitHub access must include a repository before Claude can push to it. Check with list_repos before promising a push.
