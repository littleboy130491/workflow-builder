# Step 07: HTML Extraction (Existing Site) — Instructions

## Objective

Extract and store the HTML source code of all core pages for structural analysis.

## Process

1. Read core pages from `outputs/03-core-pages/core-pages.md`

2. For each core page:
   - Fetch the full HTML source
   - Save complete HTML to `outputs/07-html-extraction/{page-name}-{priority}.html`
   - If page uses external stylesheets, note this but still save inline styles if found
   - Preserve original formatting where possible

3. For each page, also create a brief summary in `outputs/07-html-extraction/summaries/{page-name}.md`:
   - Page title and meta description
   - Key structural elements (header, nav, main sections, footer)
   - Notable JavaScript libraries or frameworks detected
   - Any inline scripts that affect rendering

4. If a page fails to fetch:
   - Note in `outputs/07-html-extraction/failed-pages.md`
   - Continue with remaining pages

## Notes

- Use view-source or DevTools to get clean HTML
- Some sites may block direct fetching — use appropriate headers (user-agent)
- Focus on semantic structure — class names, IDs, and overall document structure
