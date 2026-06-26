## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-06-26 - Prevent screen reader issues with empty badge links
**Learning:** Wrapping visual elements like badges in empty links (e.g., `[![alt](src)]()`) causes screen readers to announce them confusingly as empty links and can reload the page when clicked by users. Additionally, it violates markdown linting rules (MD042).
**Action:** Always embed static visual elements (like status badges) using plain image tags (e.g., `![alt](src)`) unless they are intended to link to a valid, meaningful destination.
