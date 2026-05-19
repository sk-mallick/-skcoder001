## 2024-05-19 - [Lazy Loading Markdown Images]
**Learning:** Found a performance bottleneck in static documentation where many large, off-screen images (like GitHub stats/graphs) were loading synchronously on page load.
**Action:** Always add `loading="lazy"` to `<img>` tags for images below the fold in documentation files like `README.md` to prevent unnecessary data usage and improve initial load speed.
