# Performance Learnings

## 2024-10-24 - Optimizing GitHub Profile Assets

**Learning:** Profile readmes can suffer from slow load times due to third-party widget cold starts (e.g., Heroku) and unnecessary 302 redirects from GitHub Blob URLs.
**Action:** Use Vercel/Cloudflare-backed endpoints (e.g., Demolab) for widgets and direct raw.githubusercontent.com URLs for images to eliminate latency.
