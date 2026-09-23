# AGENTS.md

## Project overview
Fertilizer registration app for [company]. Thai-language UI, mobile-first,
built as self-contained HTML/CSS/JS (no build step) matching Figma mockups
in `/design/`.

## Setup
- No install step — open the .html file directly in a browser.
- If a build step is added later, document the exact commands here.

## Code style
- Vanilla JS only, no framework unless explicitly requested.
- Keep CSS in a single `<style>` block; no external stylesheets.
- Use CSS custom properties (`--var`) for all colors — never hardcode
  hex values inline.
- Thai UI text stays in Thai; code comments and variable names in English.
- 2-space indentation.

## Design fidelity
- When implementing a Figma frame, match spacing, color, and type exactly
  before adding functionality — pixel-match first, wire up behavior second.
- If a Figma link/frame can't be accessed, ask for a screenshot/export
  rather than guessing at the design.
- Reuse existing design tokens (colors, radii, spacing) already defined
  in the stylesheet instead of introducing new ones.

## Testing / verification
- After any UI change, describe what was changed and why in the response —
  don't just say "done."
- For interactive flows (forms, multi-step screens), manually trace the
  happy path before considering the task complete.

## Boundaries
- Don't introduce a bundler, package.json, or new dependencies without
  asking first — this project is intentionally build-step-free.
- Don't rewrite unrelated screens/files while fixing one screen.
- Ask before changing copy/wording in the Thai UI — don't auto-translate
  or "improve" phrasing