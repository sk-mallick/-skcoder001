# Performance Learnings

## 2024-10-24 - Heroku Cold Starts in README Widgets

**Learning:** Using Heroku-backed endpoints (like `github-readme-streak-stats.herokuapp.com`) for GitHub profile README widgets can cause significant rendering latency due to Heroku's cold start behavior.

**Action:** Prefer edge-backed endpoints (e.g., Cloudflare/Vercel-backed `streak-stats.demolab.com`) to ensure fast, reliable rendering without cold start delays.
