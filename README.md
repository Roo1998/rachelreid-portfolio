# Rachel Reid: portfolio

My product design portfolio, live at **[rachelreid.vercel.app](https://rachelreid.vercel.app)**.

I designed it and built it with [Claude Code](https://claude.com/claude-code) on [Astro](https://astro.build). The type scale, colour tokens, spacing and components are my own. It's the same way I work day to day: I make the design decisions and direct Claude to build them in code, then review every change.

## What's inside

- `src/styles/global.css`: design tokens for colour, type and spacing, with a dark theme that follows the system setting
- `src/layouts`: the base page and the case study template (summary card, hero, sections, next link)
- `src/pages`: the homepage, About, CV and four case studies
- `src/pages/archive`: earlier and student work, generated from `src/data`
- `src/components/KeyTerms.astro`: a glossary component used in the lender research case study

## Accessibility

The site targets WCAG 2.1 AA:

- Text and interactive colours meet AA contrast in light and dark themes
- Visible focus styles, a skip link and keyboard access throughout, including scrollable regions
- Every content image has alt text, and embeds have descriptive titles
- Layouts reflow down to 320px wide with no horizontal scrolling
- Motion respects `prefers-reduced-motion`

Pages are checked with [axe-core](https://github.com/dequelabs/axe-core) in both themes, at desktop and phone widths.

## Run it locally

```
npm install
npm run dev
```
