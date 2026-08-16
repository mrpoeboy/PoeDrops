# PoeDrops

A single-page storefront for **PoeDrops**, a boutique laptop retailer that sells inspected machines in limited, numbered "drops." Each unit ships with its own engineering-style inspection blueprint — the idea the whole design is built around.

## Files

- `poedrops.html` — the complete site. One self-contained file: HTML, CSS, and JS all inline. No build step, no dependencies to install.

## Running it

Just open `poedrops.html` in a browser, or drop it on any static host (Netlify, Vercel, GitHub Pages, S3, etc.) — it needs nothing else to work.

## What's inside

- **Nav** — fixed header with mobile menu toggle
- **Hero** — blueprint-style SVG illustration of a laptop with annotated callouts
- **Trust strip** — inspection / shipping / returns / warranty
- **Current Drop** — product grid (4 sample laptops)
- **Process** — four-stage "how a drop is drafted" section
- **The Standard** — detailed spec breakdown with a second blueprint drawing
- **Newsletter** — email capture for drop announcements
- **Footer**

## Design system

| Token | Value | Use |
|---|---|---|
| `--deep-blue` | `#0A1B3D` | Primary background / headline text |
| `--blue-mid` | `#122A55` | Secondary panels |
| `--blue-panel` | `#0E2247` | Trust strip |
| `--line-blue` | `#4E7AB5` | Blueprint lines, accents |
| `--light-blue` | `#E3ECF8` | Light section backgrounds |
| `--white` | `#FFFFFF` | Base white |
| `--gold` | `#B99A5B` | Single warm accent (CTAs, fig. numbers) |

Fonts: **Newsreader** (serif, headlines) · **Inter** (body) · **IBM Plex Mono** (specs, labels, technical text) — loaded from Google Fonts via CDN link in `<head>`.

## Known placeholders (swap before launch)

- Product names, specs, and prices in the "Current Drop" grid
- Copy throughout (hero, process steps, spec sheet, footer links)
- Newsletter form doesn't actually submit anywhere — wire it to an email service (Mailchimp, ConvertKit, etc.)
- "Add to cart" links are non-functional — no cart/checkout logic yet
- Nav links point to on-page anchors only; `Past Drops`, `Trade In`, `Warranty`, `Shipping`, `Returns`, `Contact` have no destination pages yet

## Accessibility & responsiveness

- Keyboard focus states on all interactive elements
- Respects `prefers-reduced-motion`
- Responsive breakpoints at 980px and 720px, down to mobile
