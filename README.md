# PoeDrops Electronics

A single-page storefront for **PoeDrops Electronics** — laptops, computer accessories, external drives, system units, graphics cards, bags and chargers, with locations in Ayeduase, Bantama, and UCC Campus.

## Files

```
poedrops.html          the complete website
images/
  icon.png              your logo mark (used in the nav & footer)
  logo.png               full logo lockup (not currently placed, kept for reuse)
  hero-laptops.png        product photo used in the hero
  laptop-1.jpg … laptop-6.jpg   ← ADD YOUR OWN PHOTOS HERE
```

Keep the `images` folder in the same location as `poedrops.html` — the page links to it by relative path.

## Adding your featured laptop photos

This is the main thing you asked for. In the **Featured Laptops** section, each of the 6 cards is already wired to look for a photo:

1. Take a photo of the laptop.
2. Save it into the `images` folder, named exactly `laptop-1.jpg` (then `laptop-2.jpg`, `laptop-3.jpg`, and so on up to `laptop-6.jpg`).
3. Open `poedrops.html` in a browser — the photo appears automatically.

Until a file exists, that card shows a neat "Photo coming soon" placeholder instead of a broken image, so the page always looks tidy.

To update the name, specs, and price under a photo: open `poedrops.html` in any text editor, search for `FEATURED LAPTOPS`, and edit the text inside each card (`Laptop Name`, the spec lines, and `GH₵ ---`).

Need more than 6 cards? Copy one whole `<div class="laptop-card">…</div>` block and paste it into the grid, then update its photo filename and text.

## Running it

Just open `poedrops.html` in a browser, or upload the whole folder (html file + images folder) to any static host (Netlify, Vercel, GitHub Pages, etc.).

## Design system

Colors were pulled directly from your logo and ad:

| Token | Value | Use |
|---|---|---|
| `--navy-1` | `#050F3E` | Darkest background |
| `--navy-2` | `#0B1E6E` | Buttons, mid panels |
| `--navy-3` | `#0E2A8F` | Hero gradient, headings |
| `--sky` | `#5FC0F8` | Accent text, highlights |
| `--pale` | `#EAF3FF` | Light section backgrounds |
| `--red` | `#F61400` | Primary call-to-action (matches your original "Contact" button) |

Fonts: **Newsreader** (serif, headlines) · **Inter** (body) · **IBM Plex Mono** (labels, specs) — loaded from Google Fonts.

## What's real vs. placeholder

**Real (from what you gave me):**
- Logo mark and colors
- Phone numbers: 0503 812 812, 0554 658 559 (as tel: and WhatsApp links)
- Locations: Ayeduase, Bantama, UCC Campus
- Product categories from your ad copy

**Still placeholder — edit before launch:**
- The 6 featured laptop photos, names, specs, and prices
- Location section text ("Come through and see the current stock...") — swap in real addresses/landmarks if you have them
- WhatsApp link currently points to 0503 812 812 — update if you'd rather use the other number

## Accessibility & responsiveness

- Keyboard focus states on all interactive elements
- Respects `prefers-reduced-motion`
- Responsive down to mobile, with a slide-out nav menu
