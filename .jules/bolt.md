## 2026-06-16 - Eliminate Redirect Latency and Cold Starts
**Learning:** Using `github.com/.../blob/...` with `?raw=true` for
images causes 302 redirects, and using Heroku for third-party widgets
can result in slow cold starts.
**Action:** Use `raw.githubusercontent.com` for direct file access and
Cloudflare/Vercel-backed endpoints (like `streak-stats.demolab.com`)
to avoid latency.
