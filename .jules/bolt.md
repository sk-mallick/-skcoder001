## 2024-06-14 - Optimize image and widget URLs to reduce redirect latency and cold starts
**Learning:** `github-readme-streak-stats.herokuapp.com` suffers from Heroku cold starts. Also `github.com/.../blob/...` with `?raw=true` involves 302 redirects.
**Action:** Use `streak-stats.demolab.com` for Streak Stats. Use `raw.githubusercontent.com` directly for GitHub repository files.
