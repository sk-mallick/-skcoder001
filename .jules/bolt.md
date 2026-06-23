# Performance Learnings

## 2024-06-23 - GitHub Profile README Rendering Bottlenecks

**Learning:** Using Heroku-backed endpoints (`herokuapp.com`) for widgets like
streak stats introduces significant latency due to cold starts. Similarly,
using `github.com/.../blob/...` with `?raw=true` for images causes
unnecessary 302 redirect latency.

**Action:** Always prefer Cloudflare/Vercel-backed endpoints (e.g.,
`streak-stats.demolab.com`) for widgets and direct `raw.githubusercontent.com`
URLs for images to eliminate latency and improve rendering performance.
