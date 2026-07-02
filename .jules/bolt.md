# Performance Learnings

## 2026-07-02 - Avoiding Latency in GitHub Widgets and Images

**Learning:** Using `github-readme-streak-stats.herokuapp.com` incurs Heroku
cold-start latency, and using `?raw=true` for images incurs unnecessary 302
redirect latency.

**Action:** Use Vercel/Cloudflare-backed endpoints (e.g.,
`streak-stats.demolab.com`) for widgets, and direct
`raw.githubusercontent.com` URLs for embedding GitHub files to improve load
performance.
