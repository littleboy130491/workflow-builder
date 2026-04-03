# Step 02: Sitemap Discovery — Instructions

## Objective

Find and parse the website's sitemap to understand the full site structure.

## Process

1. Read the target URL from `outputs/01-url-intake/website-url.txt`

2. Attempt to fetch the sitemap from common locations:
   - `{domain}/sitemap.xml`
   - `{domain}/sitemap-index.xml`
   - `{domain}/wp-sitemap.xml` (WordPress)
   - `{domain}/sitemap_index.xml`

3. If sitemap is found:
   - Save raw XML to `outputs/02-sitemap/sitemap.xml`
   - Parse and convert to Markdown format in `outputs/02-sitemap/sitemap-parsed.md`
   - Include: URL, last modified date, change frequency, priority (if available)

4. If no sitemap found:
   - Attempt to discover pages by crawling the homepage and extracting links
   - Save discovered URLs to `outputs/02-sitemap/discovered-pages.txt`
   - Note the limitation in `outputs/02-sitemap/sitemap-parsed.md`

## Notes

- Some sites may require user-agent customization to access sitemap
- If blocked, fall back to manual page discovery
- Preserve URL structure for later analysis
