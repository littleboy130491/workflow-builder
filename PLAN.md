# Website Redesign Workflow Plan

## Overview

This workflow handles the initial discovery, analysis, planning, and mockup phase of a website redesign project. The goal is to capture existing website structure, identify business-critical pages, analyze visual and content weaknesses/gaps, devise an improvement plan, and generate a deployable HTML mockup.

## Workflow Structure

### Phase 1: Discovery (Input Gathering)

#### Step 01: URL Intake
- **Purpose**: Collect user-provided website URL and optional reference sites
- **Input**: Website URL, optional reference URLs
- **Output**: `outputs/01-url-intake/`

#### Step 02: Sitemap Discovery
- **Purpose**: Find and parse the website sitemap
- **Input**: Website URL from step 01
- **Output**: `outputs/02-sitemap/`
- **Action**: AI agent fetches sitemap.xml, parses structure

#### Step 03: Core Pages Identification
- **Purpose**: Determine which pages are critical for the business
- **Input**: Sitemap from step 02
- **Output**: `outputs/03-core-pages/`
- **Action**: AI analyzes sitemap to identify high-priority pages (home, about, contact, products/services, etc.)

#### Step 04: Reference Identification
- **Purpose**: Find reliable reference sites if not provided by user
- **Input**: User-provided references (if any) from step 01
- **Output**: `outputs/04-reference-sites/`
- **Action**: If no reference provided, AI researches and identifies best-in-class reference sites across perspectives:
  - **Design references**: Visual design, layout, typography, color, imagery
  - **Content references**: Copy, messaging, structure, tone
  - **User Flow references**: Navigation, CTAs, forms, conversion patterns
  - **Technical references**: Performance, accessibility, SEO best practices
  - *Note: Multiple references per perspective are acceptable*

#### Step 05: Screenshot Capture (Existing Site)
- **Purpose**: Visual documentation of existing website core pages
- **Input**: Core pages from step 03
- **Output**: `outputs/05-screenshots/`
- **Action**: Capture screenshots of each core page

#### Step 06: Screenshot Capture (References)
- **Purpose**: Visual documentation of reference sites
- **Input**: Reference sites from step 04
- **Output**: `outputs/06-reference-screenshots/`
- **Action**: Capture screenshots from reference sites by perspective (design, content, user flow, technical)

#### Step 07: HTML Extraction (Existing Site)
- **Purpose**: Extract and store HTML source of existing site
- **Input**: Core pages from step 03
- **Output**: `outputs/07-html-extraction/`
- **Action**: Copy HTML source code for core pages

#### Step 08: HTML Extraction (References)
- **Purpose**: Extract and store HTML source of reference sites
- **Input**: Reference sites from step 04
- **Output**: `outputs/08-reference-html/`
- **Action**: Copy HTML source code for reference pages

---

### Phase 2: Analysis

#### Step 09: Page Analysis (Existing Site)
- **Purpose**: Analyze existing pages for weaknesses, gaps, and strengths
- **Input**: Screenshots from step 05, HTML from step 07
- **Output**: `outputs/09-page-analysis/`
- **Action**: AI reviews each core page visually and structurally to identify:
  - **Strengths**: What's working well, good design patterns, effective content
  - **Weaknesses**: Usability issues, outdated design, poor navigation, slow loading elements
  - **Gaps**: Missing features, content gaps, unaddressed user needs, accessibility issues

#### Step 10: Reference Analysis
- **Purpose**: Analyze reference sites to understand best practices per perspective
- **Input**: Screenshots from step 06, HTML from step 08
- **Output**: `outputs/10-reference-analysis/`
- **Action**: AI analyzes reference sites by perspective:
  - **Design**: What makes their visual design effective
  - **Content**: How they structure messaging and copy
  - **User Flow**: How they guide users through conversion
  - **Technical**: Performance and accessibility patterns

---

### Phase 3: Planning

#### Step 11: Improvement Plan
- **Purpose**: Devise a comprehensive plan based on existing site analysis and reference best practices
- **Input**: Page analysis (step 09), Reference analysis (step 10)
- **Output**: `outputs/11-improvement-plan/`
- **Action**: Create actionable improvement recommendations:
  - Design improvements (layout, typography, color, imagery) — with reference examples
  - Content improvements (copy, messaging, structure) — with reference examples
  - UX improvements (navigation, CTAs, forms, user flows) — with reference examples
  - Technical improvements (performance, SEO, accessibility) — with reference examples
  - Priority ranking of all recommendations

---

### Phase 4: Mockup

#### Step 12: HTML Mockup Generation
- **Purpose**: Build deployable HTML mockup implementing the improvement plan
- **Input**: Improvement plan (step 11), Reference analysis (step 10), Reference screenshots (step 06)
- **Output**: `outputs/12-mockup/`
- **Action**: Use `ui-ux-pro-max` skill to generate clean, deployable HTML mockup:
  - Use `--stack html-tailwind` for HTML/Tailwind output
  - Generate design system first: `python3 <skill-path>/scripts/search.py "<product type>" --design-system -p "<project>"`
  - Apply design improvements from the plan
  - Implement improved layout, typography, color scheme
  - Structure content according to improved messaging
  - Include responsive design for mobile/desktop
  - Output should be self-contained HTML with inline CSS (no external dependencies) for easy deployment
  - Each core page produces one HTML file
  - Run UX validation: `python3 <skill-path>/scripts/search.py --domain ux` to verify accessibility/interaction quality
- **Skill**: `ui-ux-pro-max` (located at `/home/henry/.agents/skills/ui-ux-pro-max`)

---

### Final Output
All outputs consolidated into `inputs/website-analysis/` for use in subsequent redesign phases.

## Directory Structure

```
website-redesign-workflow/
├── workflows/
│   └── 01-website-analysis/
│       ├── 01-url-intake/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 02-sitemap-discovery/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 03-core-pages-identification/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 04-reference-identification/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 05-screenshot-capture/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 06-reference-screenshots/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 07-html-extraction/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 08-reference-html/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 09-page-analysis/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 10-reference-analysis/
│       │   ├── inputs.md
│       │   └── instructions.md
│       ├── 11-improvement-plan/
│       │   ├── inputs.md
│       │   └── instructions.md
│       └── 12-html-mockup/
│           ├── inputs.md
│           └── instructions.md
├── outputs/
│   ├── 01-url-intake/
│   ├── 02-sitemap/
│   ├── 03-core-pages/
│   ├── 04-reference-sites/
│   ├── 05-screenshots/
│   ├── 06-reference-screenshots/
│   ├── 07-html-extraction/
│   ├── 08-reference-html/
│   ├── 09-page-analysis/
│   ├── 10-reference-analysis/
│   ├── 11-improvement-plan/
│   ├── 12-mockup/
│   └── inputs/website-analysis/
├── resources/
│   └── website-analysis-diagram.md
├── PLAN.md
└── README.md
```

## Implementation Order

1. Create `workflows/01-website-analysis/` step folders with `inputs.md` and `instructions.md`
2. Create `outputs/` directory structure
3. Create `resources/website-analysis-diagram.md`
4. Create `inputs/website-analysis/` consolidation folder
