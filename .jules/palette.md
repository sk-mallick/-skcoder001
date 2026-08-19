## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2026-08-19 - Empty markdown links wrapping image badges

**Learning:** Wrapping image badges in empty markdown links
(`[![alt](url)]()`) creates empty, focusable anchor tags which are poor for
keyboard navigation and screen readers.

**Action:** Use standard markdown image tags (`![alt](url)`) instead of
wrapping them in empty links when the link has no target URL.
