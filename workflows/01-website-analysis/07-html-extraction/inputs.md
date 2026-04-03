# Step 07: HTML Extraction (Existing Site) — Inputs

## Upstream Dependencies

- `outputs/03-core-pages/core-pages.md` — List of identified core pages

## Required Inputs

- List of core page URLs from `outputs/03-core-pages/core-pages.md`

## Output Location

- `outputs/07-html-extraction/` — Contains HTML source for each core page
  - Filename format: `{page-name}-{priority}.html` (e.g., `homepage-p0.html`, `about-p1.html`)

## HTML Extraction Requirements

- Complete HTML source (full `<html>` to `</html>`)
- Inline CSS and JavaScript (if any)
- Include any critical inline assets
- Preserve original structure and class names
