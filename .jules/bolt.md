# Bolt Journal

## 2026-05-22 - GitHub Profile External Asset Optimization

**Learning:** External assets embedded in GitHub Profile READMEs often introduce
unnecessary latency. `github-readme-streak-stats.herokuapp.com` suffers from
Heroku cold starts, and `github.com/.../blob/...?raw=true` introduces a 302
redirect.

**Action:** Always prefer serverless/edge-hosted alternatives like
`streak-stats.demolab.com` for dynamic widgets and direct
`raw.githubusercontent.com` URLs for static repository assets to improve Time to
First Byte (TTFB) and overall profile render speed.
