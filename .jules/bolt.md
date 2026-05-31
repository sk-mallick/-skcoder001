## 2026-05-31 - Heroku Cold Start Latency
**Learning:** Heroku-hosted endpoints for GitHub widgets (like streak-stats) often suffer from significant cold start latency, blocking or delaying profile rendering.
**Action:** Replace `herokuapp.com` with Cloudflare/Vercel-backed endpoints (e.g., `streak-stats.demolab.com`) to ensure fast, reliable widget loading in profiles.
