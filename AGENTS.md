# Repository Guidelines

## Project Structure & Module Organization
- `index.html` is the single-page marketing site holding most CSS and JS inline; edit here for layout, copy, or behavior changes.
- `privacy.html`, `terms.html`, and `support.html` mirror the same styling assets—update only when policy or help content changes.
- `assets/` stores screenshots (`images/Screenshots/...`), logos, and QR codes; keep filenames descriptive (e.g., `04_meal-plan.jpg`).
- `site.webmanifest` and `favicon.ico` contain PWA metadata and icons; touch them only when branding or app identifiers shift.

## Build, Test, and Development Commands
- `python -m http.server 8080` — simple static server for local previews from the repo root.
- `npx serve .` — Node-based alternative that works well for phone testing over LAN.
- There is no bundler; refresh the browser after editing HTML/CSS to view changes immediately.

## Coding Style & Naming Conventions
- Use 4-space indentation in HTML and keep semantic wrappers (`<nav>`, `<section>`, `<footer>`). Keep inline scripts/styles compact.
- Manage palette and spacing through CSS variables defined in `:root`; add new tokens there before referencing them.
- Name screenshots with ordered numerals plus descriptors (`05_weekly-plan.png`) to stay aligned with the carousel script ordering.

## Testing Guidelines
- Run responsive checks in Chrome and Safari from 360px up to desktop widths; verify sticky nav, hero copy, and grid spacing.
- Exercise the screenshot carousel via click and swipe to ensure `navigate()` sequencing and touch handlers still work.
- Document manual QA steps in pull requests because the project does not ship with automated tests.

## Commit & Pull Request Guidelines
- Write imperative, present-tense commit messages ("Refine hero typography") and group related UI tweaks.
- PRs should summarize changes, link issue IDs, and include before/after screenshots for visual adjustments.
- Note any accessibility considerations (contrast, focus states, reduced motion) whenever interactive styles change.

## Security & Configuration Tips
- Never commit API keys or analytics tokens; reference them through the hosting platform’s environment settings if needed.
- Validate any third-party embed code (e.g., feedback widgets) on a branch before enabling it on production pages.
