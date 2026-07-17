## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-07-17 - Remove empty links from profile badges
**Learning:** Wrapping status badges or images in empty links (e.g., `[![alt](src)]()`) causes screen readers to announce them as confusing, broken links and reloads the page on click, creating a poor user experience.
**Action:** Use plain image tags (`![alt](src)`) for decorative or non-clickable badges in markdown instead of empty links.
