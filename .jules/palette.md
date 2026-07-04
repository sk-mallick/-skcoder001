# Performance Learnings

## 2024-05-15 - Missing alt attributes on dynamic GitHub profile components

**Learning:** Dynamic components inserted into markdown, such as capsule renders
and stat cards (e.g. GitHub activity graphs and streak stats), often omit `alt`
attributes. These are crucial for screen readers to properly interpret the
visual data being conveyed on a GitHub profile.
**Action:** Always verify that third-party image generation APIs (like
`capsule-render` and `github-readme-stats`) are appended with descriptive `alt`
tags when embedded via `<img>` tags in markdown documentation.

## 2024-05-24 - Avoid Empty Link Wrappers for Badges

**Learning:** Wrapping badges in empty links creates accessibility issues
as screen readers announce them confusingly and they cause page reloads.
**Action:** Use plain image tags for badges that do not require navigation.
