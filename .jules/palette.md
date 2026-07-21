## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.


## 2026-07-21 - Empty links wrapping badges

**Learning:** Wrapping images or badges in empty markdown links
(e.g., `[![alt](src)]()`) causes accessibility issues for screen readers,
which announce them confusingly, and clicking them might reload the page
unnecessarily.

**Action:** Always use plain image tags (e.g., `![alt](src)`) for badges and
images that do not serve as actionable links.
