# Performance Learnings

## 2026-07-10 - Third-party widget and image latency

**Learning:** Widgets on Heroku and GitHub blob URLs with `?raw=true` experience
slow cold starts and 302 redirects, which delays profile rendering.
**Action:** Use Cloudflare-backed endpoints (like `streak-stats.demolab.com`)
and direct `raw.githubusercontent.com` URLs for faster, consistent loading.
