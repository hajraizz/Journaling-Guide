# Journaling Guide

A warm, modern, single-page website that guides readers through the practice of journaling — from choosing a format to building a daily habit. Built with plain HTML, CSS, and JavaScript; no frameworks or dependencies required.

---

## Overview

**Journaling Guide** is a static informational website designed to feel calm, personal, and approachable. It covers everything a beginner or returning journaler needs: types of journaling, methods (digital, manual, visual), how to start, what to write, and the proven benefits of a regular practice.

---

## Features

- **Single-page architecture** — all sections live in one HTML file; JavaScript handles panel switching without page reloads
- **Sidebar + top navigation** — two complementary nav systems with active state highlighting
- **Dark mode toggle** — preference persisted in `localStorage`
- **Scroll progress bar** — thin accent bar at the top of the viewport tracks reading position
- **Back to Top button** — fades in after scrolling 400px
- **Smooth panel transitions** — fade-in animation on every section switch
- **Fully responsive** — adapts cleanly across mobile, tablet, and desktop breakpoints
- **Accessible** — semantic HTML, ARIA labels, `aria-live` region, keyboard navigation on sidebar (arrow keys), skip-to-content link, and focus-visible styles
- **No frameworks** — pure HTML, CSS, and vanilla JavaScript only

---

## Sections

| Section | Description |
|---|---|
| Introduction | What journaling is and why it matters |
| Types | Six journaling styles: reflective, gratitude, bullet, creative, dream, travel |
| Digital Journaling | Tools, advantages, and tips for screen-based journaling |
| Manual Journaling | The case for pen and paper |
| Visual Journaling | Art journals, collage, mixed media |
| How to Start | A practical, no-pressure framework for building the habit |
| What to Write | Five reliable starting points when you feel stuck |
| Benefits | Psychological, emotional, and practical gains |

---

## Project Structure

```
/
├── index.html          # All HTML, CSS, and JS in one file
├── README.md           # This file
└── assets/
    ├── brownie.jpeg    # Header background image
    ├── pic1.jpeg       # Introduction panel image
    ├── notion.png      # Digital journaling panel image
    ├── writing.png     # Visual journaling panel image
    └── library.jpeg    # What to Write panel image
```

---

## Getting Started

No build step, no install, no server required.

1. Clone or download the repository
2. Place your images in the `assets/` folder (see structure above)
3. Open `index.html` in any modern browser

```bash
# Or serve locally with Python
python3 -m http.server 8000
# Then open http://localhost:8000
```

---

## Customisation

All visual tokens are defined as CSS custom properties at the top of the `<style>` block, making it easy to retheme:

```css
:root {
  --clr-accent:      #a0623a;   /* Primary accent colour */
  --clr-bg:          #f5ede3;   /* Page background */
  --clr-text:        #3d1f0a;   /* Body text */
  --font-display:    'Playfair Display', Georgia, serif;
  --font-body:       'Lato', 'Trebuchet MS', sans-serif;
}
```

Dark mode overrides follow immediately under the `body.dark` selector.

---

## Typography

| Role | Font | Source |
|---|---|---|
| Headings & display | Playfair Display | Google Fonts |
| Body & UI | Lato | Google Fonts |

Both fonts are loaded via a single `<link>` tag; no local font files needed.

---

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge). No polyfills required. Internet Explorer is not supported.

---

## External Links

The top navigation includes links to external journaling resources:

- [Notion Journaling Templates](https://www.notion.com/templates/category/journaling)
- [Journaling YouTube Channel](https://www.youtube.com/channel/UCSc_BneU9wXWNIaEbiEJq_g/videos)
- [r/Journaling on Reddit](https://www.reddit.com/r/Journaling/)

All external links open in a new tab with `rel="noopener noreferrer"`.

---

> "Journal writing is a voyage to the interior." — Christina Baldwin
