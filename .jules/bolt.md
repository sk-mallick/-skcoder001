# Performance Learnings

## 2026-07-04 - Asset Loading Latency

**Learning:** Third-party widgets hosted on Heroku suffer from severe cold start
latency, and embedding GitHub repository files using blob URLs with `?raw=true`
causes unnecessary 302 redirects.

**Action:** Prefer Cloudflare/Vercel-backed endpoints (like
streak-stats.demolab.com) over Heroku, and use direct raw.githubusercontent.com
URLs to eliminate redirect latency.
