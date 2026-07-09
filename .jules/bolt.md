# Performance Learnings

## 2026-07-09 - Markdown Image Loading Optimizations

**Learning:** Using herokuapp.com endpoints for widgets causes slow loading
due to cold starts, and using github.com/blob URLs with ?raw=true
introduces unnecessary 302 redirect latency.

**Action:** Use Cloudflare/Vercel-backed endpoints like streak-stats.demolab.com
and direct raw.githubusercontent.com URLs to improve load times.
