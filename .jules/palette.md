# UX Learnings

## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components

**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-07-12 - Empty Links Around Badges

**Learning:** Wrapping images or badges in empty markdown links
(e.g., `[![<alt>](<src>)]()`) causes accessibility issues for screen
reader users (announcing confusingly and reloading the page on click)
and triggers markdown linting errors (MD042).
**Action:** When displaying non-interactive images or badges, use plain
image tags (`![<alt>](<src>)`) without wrapping them in empty links.
