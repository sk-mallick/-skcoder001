## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2024-08-13 - Empty Markdown Links on Badges

**Learning:** Wrapping image badges in empty markdown links
(e.g., `[![alt](url)]()`) creates focusable but non-functional elements that
impair screen reader and keyboard navigation.
**Action:** Always use standard image tags (e.g., `![alt](url)`) for badges
that do not need to link anywhere.
