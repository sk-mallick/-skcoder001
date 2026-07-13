# Performance Learnings

## 2024-05-18 - Avoid Heroku Cold Starts for Widgets

**Learning:** Using herokuapp.com endpoints for widgets like GitHub Streak Stats
often results in slow load times due to Heroku cold starts.
**Action:** Prefer Cloudflare or Vercel-backed endpoints like
streak-stats.demolab.com to ensure faster response times.

## 2024-05-18 - Eliminate 302 Redirect Latency for Images

**Learning:** Embedding images from GitHub using github.com with blob and
raw=true causes unnecessary 302 redirect latency.
**Action:** Always use the direct raw.githubusercontent.com URL to fetch images
directly and improve load speed.
