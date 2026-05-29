## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.
## 2024-05-29 - Empty links wrapping badges
**Learning:** Avoid wrapping image badges or other images in empty links (`[![alt](src)]()`). This is an accessibility anti-pattern as the link is focusable for keyboard navigators and screen readers but has no valid destination, leading to confusion. It also triggers `markdownlint` rule MD042.
**Action:** Use plain markdown image tags (`![alt](src)`) for badges when they do not link to any specific URL.
