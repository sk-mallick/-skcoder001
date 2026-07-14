## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-07-14 - Empty links on badge images
**Learning:** Wrapping badges or images in empty links (`[![...](...)]()`) causes accessibility issues, as screen readers announce them confusingly and clicking them reloads the page.
**Action:** Always use plain image tags (`![...](...)`) for decorative or non-clickable badges in markdown instead of empty links to improve screen reader experience and prevent unintended page reloads.
