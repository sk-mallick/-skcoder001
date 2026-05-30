## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components
**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2024-05-30 - Empty links wrapping badges
**Learning:** Wrapping images or badges in empty links (e.g., `[![<alt>](<src>)]()`) creates accessibility issues because screen readers will announce meaningless link elements and it causes markdown linting errors (MD042). This pattern is often a leftover from copy-pasting badge code.
**Action:** Always use plain image tags (`![<alt>](<src>)`) when displaying badges or images that do not actually need to link anywhere.
