---
description: Jinja template instructions for page/component changes in this FastAPI app.
applyTo: "templates/**/*.html"
---

# Jinja Template Instructions

## Composition

- Reuse components in templates/components/ whenever possible.
- Keep shared wrappers and top-level structure in templates/base.html.
- Prefer small, composable template blocks over repeated inline markup.

## Styling

- Use utility classes already defined in app/static/css/app.css.
- If a utility class is missing, add it to CSS first before using it in templates.
- Preserve readable contrast and consistent spacing across screens.

## HTMX and Interaction

- Keep HTMX attributes explicit and easy to trace.
- Preserve server-rendered fallback behavior when possible.
- Do not rely on VS Code Simple Browser for validation; use a real browser.

## Accessibility

- Keep semantic headings and button/link semantics intact.
- Ensure forms/controls have clear labels and text remains readable.
