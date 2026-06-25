# Performance Learnings

## 2026-06-25 - Avoid Heroku Cold Starts and Redirects

**Learning:** Relying on Heroku-hosted endpoints for images causes slow page
loads due to container cold starts. In addition, using blob URLs with
'?raw=true' for GitHub assets incurs a 302 redirect, adding latency.
**Action:** Always prefer Vercel/Cloudflare-backed endpoints over Heroku for
widgets, and use direct raw.githubusercontent.com URLs for GitHub assets.
