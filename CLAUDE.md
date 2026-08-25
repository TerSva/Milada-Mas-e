# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Static one-page marketing website for "Masáže Milada" — massage therapist Milada Vondrušová, Karlovy Vary. No build tooling, no framework: a single self-contained HTML document with embedded CSS/JS.

## Files

- `index.html` — the site. Single complete document: structure + all CSS (one `<style>`, organized by commented section blocks) + all JS (one inline `<script>`). The only file that gets built/deployed.
- `design-system-2.html` — separate, read-only reference library (like Storybook) for design tokens and base component CSS. Read from, never edited, unless the user explicitly asks to change the design system itself.
- `kontext.md` — chronological decision log from earlier in the project. Historical record, not necessarily in sync with the current state of `index.html` — treat `index.html` as ground truth over kontext.md when they conflict.
- Image/icon assets at repo root (hero.jpg, o-milade.jpg, sluzby-oblicej.jpg, sluzby-telo.jpg, sluzby-access.jpg, logo.svg, menu.svg, phone-2.svg, email-2.svg, lokace-2.svg) — referenced by exact filename from `index.html`.

## Workflow rules (standing, apply every session)

- Never write/edit code without an explicit go-ahead for that specific step. A general "continue" is not permission to build — propose the step first.
- Commit and push are two separate confirmations, each explicit.
- `design-system-2.html` is a shared source of truth. Before changing anything shared, ask whether the change should be global (edit the shared definition) or local (one-off override) — never assume.
- One document, organized internally — do not split `index.html` into separate CSS/JS files.
- When sending the file to the user, referenced local images/assets don't travel with it automatically — send them alongside with exact matching filenames.

## Copy conventions

- No em dashes (—) in copy, ever.
- No decorative arrows, no AI-generic UI patterns (numbered/circled step badges, generic feature-card grids, generic pricing-list-plus-button rows).
- Formal address always capitalized: Vy/Váš/Vám/Vás (vykání s velkým V) — house rule for this site.
- Prices hidden behind a click/tap (toggle), never shown in a static visible list.

## Design tokens (from design-system-2.html)

- Colors: --dark #291B10, --dark-surface #684B23, --decor #9A7338, --cta #D4821E, --spot #FFC564, --light-surface #F6EED7, --light-bg #FCF1E5, --elevated #E6D8BC.
- Spacing: --sp-1 8px … --sp-12 96px (8/16/24/32/48/64/96).
- Radius: 18px uniform (--radius).
- Type: Fraunces (variable font) only on the Hero H1; Karla everywhere else.

## Structure of index.html

Nav (fixed, transparent → dark on scroll) → Hero (Příchod) → O Miladě (Dotek) → Služby (Proměna, price list) → Kde mě najdeš → Rezervace (Odchod, phone-first booking) → Footer.

This maps to an emotional arc (Příchod/Dotek/Proměna/Odchod) carried by copy and section rhythm, not an explicit numbered "4 steps" component (tried and rejected).

## Known fragile areas

- Section-to-section background transitions use short (48px), fixed-pixel-height gradient pseudo-elements at section boundaries — not `calc()` against a dynamically-sized (`min-height:100vh`) element, after a Safari-specific rendering artifact traced to exactly that combination.
- Scroll-linked parallax (`data-speed` attribute + `updateParallax()`) is used sparingly — a decorative parallax layer in O Miladě was removed after it caused a visible rendering seam in Safari.
