# Performance Learnings

## 2026-07-17 - Third-Party Widget Endpoints

**Learning:** Heroku-backed endpoints for README widgets
(like github-readme-streak-stats) can cause slow cold starts,
negatively impacting profile rendering performance.
**Action:** Always prefer Cloudflare/Vercel-backed endpoints
(like streak-stats.demolab.com) for embedding third-party widgets
in Markdown files.
