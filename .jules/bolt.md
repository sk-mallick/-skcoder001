# Performance Learnings

## 2024-06-20 - Markdown Asset Loading Latency

**Learning:** Relying on Heroku for third-party stats widgets can
introduce 5-10s cold start latency. Additionally, using GitHub blob
URLs with '?raw=true' introduces unnecessary 302 redirect latency.

**Action:** Use Vercel/Cloudflare-backed edge endpoints (like demolab.com)
for widgets and direct raw.githubusercontent.com URLs for GitHub assets
to improve Time to First Byte (TTFB).
