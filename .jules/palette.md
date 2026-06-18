## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-06-18 - Prevent Empty Link Wrappers for Badges
**Learning:** Wrapping images or badges in empty markdown links (e.g., `[![alt](src)]()`)
causes screen readers to announce them confusingly and creates clickable elements
that simply reload the page, creating poor UX for all users.
**Action:** Always use plain image tags (`![alt](src)`) for non-interactive visual
elements to ensure smooth screen reader experiences and prevent dead clicks.
