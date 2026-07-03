# Performance Learnings

## 2024-05-24 - Avoiding 302 Redirects and Cold Starts

**Learning:** Using `github.com/.../blob/...` URLs with `?raw=true` for images
introduces unnecessary 302 redirect latency. Similarly, third-party widgets
hosted on Heroku suffer from slow cold starts, delaying README rendering.

**Action:** Always use direct `raw.githubusercontent.com` URLs for embedding
GitHub repository files and prefer Cloudflare/Vercel-backed endpoints
(e.g., `streak-stats.demolab.com`) for dynamic widgets to ensure optimal load
times.
