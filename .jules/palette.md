## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-08-05 - Empty links on badges impair accessibility

**Learning:** Wrapping status badges in empty markdown links is a pattern used in this profile that causes screen readers to announce them confusingly and reloads the page on click.
**Action:** Always use plain image tags for badges unless they need to link to an external resource.
