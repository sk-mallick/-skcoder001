## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-07-27 - Removing empty markdown links from badges
**Learning:** Wrapping status badges or images in empty markdown links (e.g., `[![alt](src)]()`) causes accessibility issues, as screen readers announce them confusingly as blank links and clicking them reloads the page.
**Action:** Use plain markdown image tags (e.g., `![alt](src)`) for purely visual or non-interactive badges rather than wrapping them in empty links.
