# Frontend Assignment 2 — Flexbox & CSS Grid

A small multi-page website built with **plain HTML and CSS** (no JavaScript, no frameworks) to practice two core CSS layout systems: **Flexbox** and **CSS Grid**. The theme of the content is ASUS product lines (ProArt, ROG, TUF).

All five pages share a single stylesheet (`style.css`) and a common navigation bar and footer.

## Pages and tasks

| Page | File | Task | Main technique |
| --- | --- | --- | --- |
| Home | `index.html` | Landing page with navigation | Flexbox (navbar) |
| Cards | `cards.html` | **Task 1** — Card row | Flexbox |
| Layout | `layout.html` | **Task 2** — Page layout with grid areas | CSS Grid (`grid-template-areas`) |
| Gallery | `gallery.html` | **Task 3** — Image gallery | CSS Grid (`repeat(3, 1fr)`) |
| Portfolio | `portfolio.html` | **Task 4** — Portfolio page | Flexbox + Grid combined |

## Features

- **Shared navigation bar** — built with Flexbox; logo on the left, links on the right, hover colour change.
- **Cards (Flexbox)** — three equal-width cards in a row (`flex: 1`). Each card is itself a flex column, so the "Read more" buttons always stick to the bottom regardless of text length. Cards lift up with a shadow on hover.
- **Grid layout** — classic page skeleton (header, sidebar, main, footer) described visually with `grid-template-areas`.
- **Gallery (Grid)** — nine images in a responsive three-column grid. A caption fades in over the image on hover.
- **Portfolio (Flexbox + Grid)** — an outer Grid splits the page into a wide projects column and a narrow "About me" sidebar (`3fr 1fr`); inside the projects column, Flexbox stacks the project cards vertically.
## Tech stack

- HTML5 (semantic tags: `header`, `section`, `aside`, `footer`)
- CSS3: Flexbox, CSS Grid, transitions, absolute positioning, `rgb()` / `rgba()` colours
## Project structure

```
frontend-assignment-2/
├── index.html        # Home page
├── cards.html        # Task 1: card row (Flexbox)
├── layout.html       # Task 2: grid areas layout
├── gallery.html      # Task 3: image gallery (Grid)
├── portfolio.html    # Task 4: portfolio (Flexbox + Grid)
├── style.css         # Shared styles for all pages
├── photos/           # Images used on the Cards and Gallery pages
└── README.md
```

## Getting started

No installation or build step is needed.

1. Clone or download the repository:
```bash
   git clone https://github.com/nursultan-duisenbek/frontend-assignment-2.git
```
2. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari).
3. Use the navigation bar at the top to move between pages.
## Design notes

| Colour | Usage |
| --- | --- |
| `#39502c` (dark green) | Navbar, footer, buttons, card borders |
| `#677e67` (muted green) | Page background |
| `#222` | Body text |
| `#fff` | Text on dark backgrounds |
| `rgb(246 239 149)` (soft yellow) | Navigation link hover |

The four coloured blocks on the Layout page (`#3498db`, `#9b59b6`, `lightpink`, `aquamarine`) are intentionally bright so the grid areas are easy to tell apart.

## Known limitations / possible improvements

- No responsive breakpoints yet (`@media` queries) — on narrow screens the three cards and the gallery stay in columns.
- Buttons ("Read more", "View") are visual only and do not link anywhere.
- Hover effects (card lift, gallery captions) do not apply on touch screens.
## Live demo

[Add your GitHub Pages / Netlify link here after publishing]

## Author

Duisenbekuly Nursultan, group SE-2524
 

