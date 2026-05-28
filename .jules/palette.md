## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-05-28 - Empty links wrapping images
**Learning:** Wrapping images (like badges) in empty links (e.g., `[![alt](src)]()`) creates interactive elements without valid targets. This is confusing for both mouse users (who see a pointer cursor but can't click anywhere) and screen reader users (who encounter broken or meaningless links).
**Action:** Use plain image tags (`![alt](src)`) instead of empty link wrappers when the image does not need to navigate anywhere.
