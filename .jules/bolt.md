## 2026-06-15 - Optimize Markdown Asset Loading
**Learning:** Using `github-readme-streak-stats.herokuapp.com` causes slow
Heroku cold starts, and using `github.com/.../blob/...?raw=true` for GitHub
files incurs unnecessary 302 redirect latency.
**Action:** Prefer Cloudflare/Vercel-backed endpoints (e.g.,
`streak-stats.demolab.com`) for streak stats and direct
`raw.githubusercontent.com` URLs for GitHub repository files to eliminate
latency.
