# Performance Learnings

## 2026-06-21 - Avoid Heroku Cold Starts

**Learning:** Heroku-hosted widgets can introduce significant latency
due to cold starts.

**Action:** Prefer Cloudflare or Vercel-backed endpoints (e.g., Demolab)
for GitHub profile widgets to ensure fast loading times.
