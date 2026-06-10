## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2024-06-10 - Avoiding Empty Links for Images and Badges
**Learning:** Wrapping images or badges in empty links (e.g., `[![<alt>](<src>)]()`) causes accessibility issues for screen readers as they try to read the empty link, and triggers markdown linting errors (MD042). Plain image tags should be used instead.
**Action:** Avoid wrapping badges or images in empty links and use plain image tags (`![<alt>](<src>)`) instead.
