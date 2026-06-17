## 2024-06-17 - Avoid Heroku Cold Starts and 302 Redirects
**Learning:** Using Heroku-backed widgets causes 2-3s cold
starts, and using github.com/blob with ?raw=true causes 302 redirect
latency. Cloudflare-backed domains and raw.githubusercontent.com
provide faster responses.
**Action:** Use streak-stats.demolab.com for stats widgets
and raw.githubusercontent.com for images to eliminate unnecessary
latency.
