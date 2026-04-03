# Step 12: HTML Mockup Generation — Inputs

## Upstream Dependencies

- `outputs/11-improvement-plan/improvement-plan.md` — Comprehensive improvement plan
- `outputs/10-reference-analysis/` — Reference best practices
- `outputs/06-reference-screenshots/` — Reference screenshots
- `outputs/05-screenshots/` — Existing site screenshots
- `outputs/09-page-analysis/` — Page analyses

## Required Inputs

- Improvement plan with prioritized recommendations
- Reference analysis by perspective
- Screenshots of existing site and references

## Output Location

- `outputs/12-mockup/` — Contains generated HTML mockup files
  - `index.html` — Homepage mockup
  - `{page-name}.html` — Additional page mockups
  - `styles.css` — Shared styles (if needed)
  - `mockup-guide.md` — Documentation for the mockup

## Skill

- **Skill Name**: `ui-ux-pro-max`
- **Skill Path**: `/home/henry/.agents/skills/ui-ux-pro-max`
- **Stack**: `--stack html-tailwind`

## Mockup Requirements

- Self-contained HTML with inline CSS (no external dependencies)
- Easy to deploy (open in browser to view)
- Responsive design (mobile + desktop)
- Applies all improvements from the plan
