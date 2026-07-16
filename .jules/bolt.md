# Performance Learnings

## 2026-07-16 - Avoiding Slow Image Loads

**Learning:** Using github.com blob URLs with raw=true for images introduces slow 302 redirects, and Heroku-backed widget endpoints suffer from slow cold starts which degrade profile rendering performance.
**Action:** Always use direct raw.githubusercontent.com URLs for GitHub repository files and prefer Cloudflare/Vercel-backed endpoints (e.g., streak-stats.demolab.com) for third-party widgets.
