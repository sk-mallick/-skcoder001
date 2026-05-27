## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-05-27 - Empty Links Around Badges
**Learning:** Wrapping images or badges in empty links (e.g., `[![alt](src)]()`) creates focusable elements that do nothing, frustrating keyboard and screen reader users, and triggers markdown linting errors (MD042).
**Action:** Use plain image tags (`![alt](src)`) when an image does not need to link anywhere.
