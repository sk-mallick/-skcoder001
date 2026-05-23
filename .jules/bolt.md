## 2024-05-24 - Avoiding Slow Heroku Cold Starts and Redirect Latency in Profile Readmes
**Learning:** Using `herokuapp.com` for streak stats APIs can introduce significant loading latency due to Heroku's cold start mechanics. Similarly, embedding images using `github.com/.../blob/...` URLs with `?raw=true` incurs unnecessary 302 redirect latency.
**Action:** Always prefer Cloudflare/Vercel-backed endpoints (e.g., `streak-stats.demolab.com`) over Heroku endpoints. Always use `raw.githubusercontent.com` URLs to directly access file assets to avoid 302 redirects.
