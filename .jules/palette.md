## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2024-05-24 - Empty Markdown Links on Image Badges

**Learning:** Empty markdown links (e.g. `[![alt](url)]()`) create focusable interactive elements that lead nowhere, creating a confusing experience for screen reader users and keyboard navigators. These are commonly copy-pasted as placeholders for status badges.
**Action:** Always replace empty wrapper links around images with simple image tags (`![alt](url)`) unless they need to point to a specific destination.
