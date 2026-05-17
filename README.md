# AI JD Portfolio Workflow

A reusable workflow for turning a job description, an experience knowledge base, and external design references into tailored resume/portfolio pages.

This repository is intentionally generic. It does not include any personal resume, private company information, screenshots, contact details, or proprietary materials.

## What It Does

1. Captures reusable experience facts into structured cards.
2. Breaks down a JD into explicit and hidden requirements.
3. Selects the strongest matching experience modules.
4. Extracts design direction from reference websites.
5. Produces a Markdown resume and an HTML portfolio version.
6. Verifies the HTML output with browser screenshots.

## Integrated Open Source Tools

### brandmd

- Repository: https://github.com/yuvrajangadsingh/brandmd
- License: MIT
- Role: extract design tokens and a `DESIGN.md` from reference websites.

### screenshot-to-code

- Repository: https://github.com/abi/screenshot-to-code
- License: MIT
- Role: optional screenshot-to-layout/code drafting for specific sections.

This workflow references those tools instead of vendoring their source code.

## Recommended Folder Structure

```text
.
├── docs/
│   ├── workflow.md
│   ├── design-reference-pipeline.md
│   └── safety-and-privacy.md
├── templates/
│   ├── experience-card.md
│   ├── jd-analysis.md
│   ├── portfolio-brief.md
│   └── copywriting-principles.md
├── examples/
│   └── demo-jd.md
└── scripts/
    └── README.md
```

## Workflow Summary

1. Save the JD into `inputs/jd/`.
2. Update experience cards in `inputs/experience/`.
3. Run JD analysis using `templates/jd-analysis.md`.
4. Extract design references with `brandmd`.
5. Optionally generate layout drafts from screenshots.
6. Write a portfolio brief.
7. Generate Markdown and HTML outputs.
8. Run browser screenshots and visual QA.

## Privacy Rule

Keep personal information out of this repo. Treat this as a public workflow template, not as a resume archive.

