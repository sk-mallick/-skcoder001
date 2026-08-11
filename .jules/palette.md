## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2024-05-16 - Empty anchor tags wrapping badge images

**Learning:** Image badges wrapped in empty anchor tags
(e.g., `[![alt](url)]()`) create focusable links that lead nowhere, causing
confusion and poor UX for keyboard and screen reader users.

**Action:** Remove the empty markdown link wrapper and use standard markdown
image tags instead to improve keyboard accessibility.
