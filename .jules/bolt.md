# Performance Learnings

## 2026-06-26 - Image Load Latency on GitHub Profiles

**Learning:** Widgets hosted on Heroku suffer from slow cold starts. Using
`?raw=true` for GitHub blobs causes unnecessary 302 redirects, degrading
load performance.
**Action:** Use Vercel/Cloudflare-backed alternatives (like
`streak-stats.demolab.com`) and direct `raw.githubusercontent.com` URLs.
