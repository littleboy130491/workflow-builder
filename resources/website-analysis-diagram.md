# Workflow Diagram

Website Redesign — Discovery, Analysis & Mockup

## Phase 1: Discovery (Input Gathering)

```mermaid
flowchart TD
    subgraph D1["Phase 1: Discovery"]
        A[01-url-intake: Collect URL & references]
        B[02-sitemap-discovery: Find sitemap]
        C[03-core-pages-identification: Identify critical pages]
        D[04-reference-identification: Find reference sites]
        E[05-screenshot-capture: Capture existing site screenshots]
        F[06-reference-screenshots: Capture reference screenshots]
        G[07-html-extraction: Extract existing site HTML]
        H[08-reference-html: Extract reference HTML]
    end

    A --> B
    B --> C
    C --> D
    D --> E
    D --> F
    E --> G
    F --> H
    D --> H
```

## Phase 2: Analysis

```mermaid
flowchart TD
    subgraph A2["Phase 2: Analysis"]
        I[09-page-analysis: Analyze existing site]
        J[10-reference-analysis: Analyze references]
    end

    G[I] --> I
    E[I] --> I
    H[J] --> J
    F[J] --> J
```

## Phase 3: Planning

```mermaid
flowchart TD
    subgraph A3["Phase 3: Planning"]
        K[11-improvement-plan: Create improvement plan]
    end

    I[K] --> K
    J[K] --> K
```

## Phase 4: Mockup

```mermaid
flowchart TD
    subgraph A4["Phase 4: Mockup"]
        L[12-html-mockup: Generate deployable HTML]
    end

    K[L] --> L
    J[L] --> L
```

## Full Flow

```mermaid
flowchart TD
    A[01-url-intake: Collect URL & references]
    B[02-sitemap-discovery: Find sitemap]
    C[03-core-pages-identification: Identify critical pages]
    D[04-reference-identification: Find reference sites]
    E[05-screenshot-capture: Capture existing site]
    F[06-reference-screenshots: Capture reference screenshots]
    G[07-html-extraction: Extract existing site HTML]
    H[08-reference-html: Extract reference HTML]
    I[09-page-analysis: Analyze existing site]
    J[10-reference-analysis: Analyze references]
    K[11-improvement-plan: Create improvement plan]
    L[12-html-mockup: Generate deployable HTML]

    A --> B
    B --> C
    C --> D
    D --> E
    D --> F
    E --> G
    F --> H
    G --> I
    E --> I
    H --> J
    F --> J
    I --> K
    J --> K
    K --> L

    style A fill:#e1f5fe
    style B fill:#e1f5fe
    style C fill:#e1f5fe
    style D fill:#e1f5fe
    style E fill:#e1f5fe
    style F fill:#e1f5fe
    style G fill:#e1f5fe
    style H fill:#e1f5fe
    style I fill:#fff3e0
    style J fill:#fff3e0
    style K fill:#e8f5e9
    style L fill:#f3e5f5
```

## Outputs

| Step | Output Directory | Description |
|------|------------------|-------------|
| 01 | `outputs/01-url-intake/` | Website URL and user references |
| 02 | `outputs/02-sitemap/` | Parsed sitemap structure |
| 03 | `outputs/03-core-pages/` | Prioritized core pages list |
| 04 | `outputs/04-reference-sites/` | Reference sites by perspective |
| 05 | `outputs/05-screenshots/` | Existing site screenshots |
| 06 | `outputs/06-reference-screenshots/` | Reference site screenshots |
| 07 | `outputs/07-html-extraction/` | Existing site HTML source |
| 08 | `outputs/08-reference-html/` | Reference site HTML source |
| 09 | `outputs/09-page-analysis/` | Existing site analysis |
| 10 | `outputs/10-reference-analysis/` | Reference best practices |
| 11 | `outputs/11-improvement-plan/` | Improvement recommendations |
| 12 | `outputs/12-mockup/` | Deployable HTML mockups |
