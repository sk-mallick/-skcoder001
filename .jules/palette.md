## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-06-14 - Prevent empty links around images
**Learning:** Wrapping images or badges in empty links
(e.g., `[![<alt>](<src>)]()`) causes accessibility issues for screen
readers (which announce them confusingly and reload the page on click)
and triggers markdownlint MD042 errors.
**Action:** Use plain image tags instead (`![<alt>](<src>)`) when
embedding badges or images in GitHub markdown profiles.
