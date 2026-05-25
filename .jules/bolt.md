## 2026-05-25 - [GitHub Profile README Optimizations]
**Learning:** Legacy widgets (e.g., herokuapp.com streak stats) introduce cold start latency (3-5s). Using blob paths with `?raw=true` for internal images induces 302 redirects.
**Action:** Always prefer Vercel/Cloudflare edge endpoints (like `demolab.com`) for widgets, and direct `raw.githubusercontent.com` URLs for hosted repo assets to bypass latency and redirects.
