# Apartman 347 — Project Instructions

## Project Overview
Static single-page website for a vacation rental apartment in Pec pod Sněžkou, Czech Republic.
- **File**: `index.html` (single file — all HTML, CSS, and JS inline)
- **Language**: Czech (with English toggle via JS)
- **Deploy**: Git → GitHub → Vercel (auto-deploy)

## Tech Stack
- Plain HTML/CSS/JS — no build step, no framework
- Google Fonts: Playfair Display (headings), Inter (body)
- `node_modules/sharp` — used for local image processing scripts only (not served)

## Design System
| Token | Value | Use |
|---|---|---|
| `--dark` | `#2a2a1e` | Backgrounds, nav, text |
| `--olive` | `#4a4a2c` | Accents, labels |
| `--cream` | `#f4efe6` | Light section backgrounds |
| `--gold` | `#c9a84c` | Highlights, numbers |
| `--airbnb` | `#FF5A5F` | CTA buttons |
| `--text-muted` | `#6b6b50` | Body text |

## Page Sections (in order)
1. `nav` — fixed, transparent → dark on scroll, hamburger mobile menu, language switch (CS/EN)
2. `.hero` — full-height bg image, headline, CTA buttons, stats bar
3. `.highlights` — icon strip (dark bg)
4. `.about` — 2-col grid (image + text + feature list)
5. `.gallery` — tabbed grid with lightbox, 4-col layout
6. `.amenities` — card grid on dark bg
7. `.stats-section` — 4-col stats on olive bg
8. `.guide` — tabbed local area guide with cards
9. Reviews section — real Airbnb reviews (124 total, 4.94 rating)
10. `footer`

## Images
- Stored in `fotky/` directory (Czech filenames, some spaces)
- Newer photos in `fotky/Nové 2020/Nové 2020/`
- Logo variants in `logo/`

## Key Constraints
- All content in Czech + English (language switcher via JS `data-cs`/`data-en` attributes)
- Maintain olive/cream/gold/dark color palette — do not introduce new colors
- Airbnb red (`#FF5A5F`) is reserved for Airbnb CTAs only
- Mobile-optimized (hamburger nav, responsive grid breakpoints)
