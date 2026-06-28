# Performance Learnings

## 2026-06-28 - Avoid Heroku Cold Starts and Redirect Latency

**Learning:** Using herokuapp.com for GitHub README badges causes slow
rendering due to cold starts. Also, embedding github.com/blob URLs with
?raw=true introduces unnecessary 302 redirects.

**Action:** Use Vercel/Cloudflare-backed demolab.com endpoints for badges and
direct raw.githubusercontent.com URLs for images to minimize latency.
