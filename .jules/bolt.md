## 2026-06-06 - Image Loading Optimizations
**Learning:** GitHub raw blob URLs and Heroku-hosted widgets cause significant loading delays (302 redirects and cold starts) in markdown profiles.
**Action:** Use `raw.githubusercontent.com` direct links and Cloudflare/Vercel-backed endpoints (like `demolab.com`) to minimize latency.
