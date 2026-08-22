## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2026-08-22 - Empty Markdown Links Create Accessibility Issues

**Learning:** Empty markdown links wrapping static badges create unnecessary,
focusable anchor tags that confuse keyboard and screen reader users by leading
nowhere.
**Action:** When adding static badges, use standard image tags instead of
wrapping them in empty markdown links to maintain a clean tab order.
