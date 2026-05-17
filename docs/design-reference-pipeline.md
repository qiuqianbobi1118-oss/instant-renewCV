# Design Reference Pipeline

Use this pipeline to learn from reference websites without copying them directly.

## Tool 1: brandmd

`brandmd` extracts design systems from URLs.

```bash
npx brandmd https://example.com -o references/example-DESIGN.md
npx brandmd https://example.com --json > references/example.tokens.json
npx brandmd https://example.com --html > references/example-brand-guide.html
```

Use it for:

- Color palettes.
- Typography rules.
- Spacing scale.
- Border radius.
- Shadow patterns.
- Component patterns.
- Overall design language.

Do not use it to copy another brand identity wholesale.

## Tool 2: screenshot-to-code

`screenshot-to-code` can turn a screenshot into draft UI code.

Use it for:

- Understanding difficult layout structure.
- Testing section composition ideas.
- Generating disposable drafts.

Do not use it as the final source of truth.

Recommended flow:

1. Capture a screenshot.
2. Generate a draft layout.
3. Extract the structural idea.
4. Rewrite the section using your own content and design system.

## AI Agent Brief

When passing design references to an AI coding agent, include:

- `DESIGN.md`.
- 2-4 screenshots.
- Current page file.
- Content source.
- Privacy constraints.
- What to preserve.
- What to change.

Example:

```text
Use references/example-DESIGN.md for palette, spacing, rhythm, and component language.
Do not copy text, images, logos, or exact layout.
Rebuild the candidate portfolio page using our content and public-safe language.
```

