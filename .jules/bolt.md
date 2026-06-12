## 2026-06-12 - Avoid 302 Redirect Latency & Heroku Cold Starts
**Learning:** Using github.com blob URLs for images incurs an
unnecessary 302 redirect, and Heroku-hosted streak stats suffer from slow
cold starts.
**Action:** Always use raw.githubusercontent.com for direct repository
file embeddings and Cloudflare/Vercel-backed endpoints (like
streak-stats.demolab.com) for third-party widgets in static repos.
