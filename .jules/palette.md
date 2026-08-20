## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2024-05-16 - Empty markdown link wrappers around badges
**Learning:** Wrapping image badges in empty markdown links (e.g., `[![alt](url)]()`) creates empty, focusable anchor tags in the generated HTML. This causes screen readers to announce an empty link, which is confusing and degrades the accessibility of the documentation.
**Action:** Remove the empty link wrappers and replace them with standard markdown image tags (e.g., `![alt](url)`) to eliminate the empty, focusable anchor link.
