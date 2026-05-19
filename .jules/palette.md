## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2024-05-14 - Removed empty wrapper links around images
**Learning:** In GitHub markdown profiles, wrapping images with empty links (like `[![<alt>](<src>)]()`) causes accessibility issues for screen readers (they announce a link that goes nowhere) and fails markdown linter rules (MD042 "No empty links").
**Action:** Always use plain image tags `![<alt>](<src>)` when you just want to display an image without linking to another resource.
