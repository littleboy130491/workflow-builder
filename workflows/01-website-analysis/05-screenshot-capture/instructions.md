# Step 05: Screenshot Capture (Existing Site) — Instructions

## Objective

Capture full-page screenshots of all core pages for visual analysis.

## Process

1. Read core pages from `outputs/03-core-pages/core-pages.md`

2. For each core page:
   - Navigate to the URL
   - Set viewport to 1920x1080 (desktop)
   - Scroll through entire page to capture full content
   - Take full-page screenshot
   - Save to `outputs/05-screenshots/` with naming convention: `{page-name}-{priority}.png`

3. Verify each screenshot:
   - Page loaded completely (no loading spinners)
   - Full content is visible (not truncated)
   - No overlay modals or popups blocking content

4. If a page fails to load:
   - Note in `outputs/05-screenshots/failed-pages.md`
   - Attempt alternative URL variations (http/https, www/no-www)
   - Continue with remaining pages

## Notes

- Use a headless browser or screenshot tool (e.g., Puppeteer, Playwright, puppeteer-screenshot, or browser extension)
- Ensure page is in final rendered state before capturing
- Keep original resolution — do not upscale
