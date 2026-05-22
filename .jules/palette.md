## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2026-05-22 - Empty links on markdown images
**Learning:** Images or badges wrapped in empty links (e.g., `[![alt](src)]()`) create "dead" focusable elements that confuse screen readers, disrupt keyboard navigation, and cause MD042 linting errors.
**Action:** Remove empty link wrappers and use plain image tags (`![alt](src)`) for badges/images that do not need to link anywhere.
