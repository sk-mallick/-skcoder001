## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2026-07-10 - Remove empty links around images

**Learning:** Wrapping images or badges in empty links
(e.g., `[![alt](src)]()`) creates accessibility issues for
screen readers and markdown linting errors.
Screen readers announce them confusingly.
**Action:** Avoid wrapping images in empty links;
use plain image tags (e.g., `![alt](src)`) instead.
