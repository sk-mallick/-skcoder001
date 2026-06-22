# UX Learnings

## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components

**Learning:** Dynamic components inserted into markdown, such as capsule renders and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt` attributes. These are crucial for screen readers to properly interpret the visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like `capsule-render` and `github-readme-stats`) are appended with descriptive `alt` tags when embedded via `<img>` tags in markdown documentation.

## 2026-06-22 - Empty links around badges cause accessibility issues

**Learning:** Wrapping images or badges in empty links (e.g.,
`[![<alt>](<src>)]()`) causes accessibility issues for screen readers,
which announce them confusingly and reload the page on click.
**Action:** Use plain image tags (e.g., `![<alt>](<src>)`) for non-navigational
badges in markdown to ensure a seamless experience for assistive
technologies.
