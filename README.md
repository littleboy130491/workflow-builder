# Website Redesign Workflow

Comprehensive workflow for discovering, analyzing, and redesigning websites. The workflow captures the existing site structure, identifies improvement opportunities using reference sites, and generates deployable HTML mockups.

## Workflow Overview

### Phase 1: Discovery (Input Gathering)

| Step | Name | Description |
|------|------|-------------|
| 01 | URL Intake | Collect target website URL and optional references |
| 02 | Sitemap Discovery | Find and parse the website sitemap |
| 03 | Core Pages Identification | Identify business-critical pages |
| 04 | Reference Identification | Find reference sites by perspective |
| 05 | Screenshot Capture (Existing) | Capture screenshots of core pages |
| 06 | Screenshot Capture (References) | Capture screenshots from reference sites |
| 07 | HTML Extraction (Existing) | Extract HTML source from core pages |
| 08 | HTML Extraction (References) | Extract HTML source from reference sites |

### Phase 2: Analysis

| Step | Name | Description |
|------|------|-------------|
| 09 | Page Analysis | Analyze existing site for strengths/weaknesses/gaps |
| 10 | Reference Analysis | Extract best practices from references |

### Phase 3: Planning

| Step | Name | Description |
|------|------|-------------|
| 11 | Improvement Plan | Create actionable recommendations with reference grounding |

### Phase 4: Mockup

| Step | Name | Description |
|------|------|-------------|
| 12 | HTML Mockup | Generate deployable HTML implementing improvements |

## Quick Start

1. **Start with Step 01**: Provide the target website URL
2. **Follow the workflow**: Complete steps in order
3. **Review outputs**: Each step produces documented outputs
4. **Generate mockup**: Step 12 produces deployable HTML

## Workflow Structure

```
workflows/
└── 01-website-analysis/
    ├── 01-url-intake/
    ├── 02-sitemap-discovery/
    ├── 03-core-pages-identification/
    ├── 04-reference-identification/
    ├── 05-screenshot-capture/
    ├── 06-reference-screenshots/
    ├── 07-html-extraction/
    ├── 08-reference-html/
    ├── 09-page-analysis/
    ├── 10-reference-analysis/
    ├── 11-improvement-plan/
    └── 12-html-mockup/
```

## Outputs Structure

```
outputs/
├── 01-url-intake/
├── 02-sitemap/
├── 03-core-pages/
├── 04-reference-sites/
├── 05-screenshots/
├── 06-reference-screenshots/
├── 07-html-extraction/
├── 08-reference-html/
├── 09-page-analysis/
├── 10-reference-analysis/
├── 11-improvement-plan/
└── 12-mockup/
```

## Skills

- **UI/UX Pro Max**: Used in Step 12 for HTML mockup generation
  - Location: `/home/henry/.agents/skills/ui-ux-pro-max`
  - Stack: HTML with Tailwind (html-tailwind)

## Diagram

See `resources/website-analysis-diagram.md` for visual representation of the workflow.
