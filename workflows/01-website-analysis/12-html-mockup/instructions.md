# Step 12: HTML Mockup Generation — Instructions

## Objective

Generate deployable HTML mockups implementing the improvement plan, using the `ui-ux-pro-max` skill.

## Skill Setup

- **Skill Path**: `/home/henry/.agents/skills/ui-ux-pro-max`
- **Stack**: HTML with Tailwind CSS (html-tailwind)
- **Design System**: Generate using `--design-system` flag

## Process

### Part 1: Generate Design System

1. Read the improvement plan to identify:
   - Product type (e.g., business website, SaaS, portfolio)
   - Industry/niche
   - Key style keywords from recommendations

2. Generate design system using the skill:
   ```bash
   python3 /home/henry/.agents/skills/ui-ux-pro-max/scripts/search.py "<product_type> <industry> <keywords>" --design-system -p "<Project Name>"
   ```

3. Review generated design system:
   - Color palette
   - Typography system
   - Style recommendations
   - Component patterns

### Part 2: Apply UX Validation

4. Run UX validation checks:
   ```bash
   python3 /home/henry/.agents/skills/ui-ux-pro-max/scripts/search.py --domain ux
   ```

5. Apply key UX rules to mockup:
   - Accessibility (contrast, alt text, keyboard nav)
   - Touch targets (minimum 44x44px)
   - Responsive breakpoints
   - Animation timing (150-300ms)

### Part 3: Generate HTML Mockups

6. For each core page from `outputs/03-core-pages/core-pages.md`:
   a. Read page analysis and improvement recommendations
   b. Read relevant reference screenshots
   c. Generate HTML implementing:
      - Design improvements (layout, typography, colors)
      - Content improvements (headlines, messaging)
      - UX improvements (navigation, CTAs)
      - Technical improvements (semantic HTML, accessibility)

7. Output requirements:
   - Self-contained HTML (inline `<style>` and `<script>`)
   - Use Tailwind-inspired utility classes
   - No external dependencies (no CDN links)
   - Mobile-first responsive design
   - Semantic HTML structure
   - Accessible (WCAG 2.1 AA)

### Part 4: Document

8. Create `outputs/12-mockup/mockup-guide.md`:
   - List of all generated files
   - Key design decisions implemented
   - How to deploy (simple — just open HTML file or host static)
   - Notes for developers

## Recommended Approach

1. Generate homepage first as the primary reference
2. Create shared styles section for common components
3. Generate remaining pages applying the same system
4. Ensure visual consistency across all pages

## Notes

- Use `--design-system` first for comprehensive guidance
- Follow the html-tailwind stack patterns from the skill
- Prioritize accessibility in every component
- Keep mockup functional — focus on key pages first (P0 pages)
- Make deployment trivial — single HTML files that just work
