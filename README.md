# Portfolio Website 🌐

A personal portfolio website with scroll-driven 3D animation, interactive elements, and a bold dark aesthetic. Built with vanilla JS + Three.js — no frameworks, no build step.

![Three.js](https://img.shields.io/badge/Three.js-r128-black) ![Vanilla JS](https://img.shields.io/badge/JS-Vanilla-yellow) ![License](https://img.shields.io/badge/license-MIT-green)

---

## Features

- **Scroll-driven 3D models** — Icosahedron, torus knot, and octahedron animate as you scroll using Three.js
- **Mouse parallax** — Camera subtly follows the cursor for depth
- **Magnetic buttons** — CTA button follows the cursor with a spring effect
- **Custom cursor** — Dot + ring cursor with hover state expansion
- **Animated card visuals** — Each project card has a live canvas animation (flow field, waveform, particles, grid)
- **Scroll reveal** — Sections fade and slide up on enter using IntersectionObserver
- **Film grain overlay** — Subtle SVG noise texture over the entire page
- **Fully responsive** — Mobile-ready layout

---

## Setup

No build step needed. Just open the file:

```bash
# Clone
git clone https://github.com/yourusername/portfolio.git
cd portfolio

# Open directly in browser
open index.html

# Or serve locally
npx serve .
# or
python -m http.server 8000
```

Then visit `http://localhost:8000`.

---

## Customization

### 1. Your name & info
In `index.html`, find and replace:
- `"Your Name"` → your actual name
- `"Creative Developer & Designer"` → your title
- `hello@yourname.com` → your email
- The hero subtitle text

### 2. Projects
Each `.project-card` block has:
- `.card-tag` — tech stack / category
- `.card-title` — project name
- `.card-desc` — short description
- `.card-link` href values — GitHub / live URLs

### 3. Skills
Update the `.skill-item` divs in the About section.

### 4. Stats
Change the `.stat-num` values (years, projects, clients).

### 5. Colors
Edit the CSS variables at the top of `<style>`:
```css
:root {
  --accent: #c8ff00;     /* lime green — change to your brand color */
  --accent2: #ff6b35;    /* orange accent */
  --bg: #04040a;         /* background */
}
```

### 6. Social links
Update the `.social-link` anchor hrefs in the contact section.

---

## Project Structure

```
portfolio/
├── index.html     # Everything — HTML, CSS, JS in one file
└── README.md
```

Single-file for easy deployment to GitHub Pages, Netlify, or Vercel.

---

## Deploy to GitHub Pages

1. Push to GitHub
2. Go to repo Settings → Pages
3. Set source to `main` branch, `/ (root)`
4. Your site is live at `https://yourusername.github.io/portfolio`

---

## Tech Used

| Tool | Purpose |
|---|---|
| Three.js r128 | 3D scene, scroll-driven models |
| Web Canvas API | Card mini-animations |
| IntersectionObserver | Scroll reveal |
| CSS Custom Properties | Theming |
| Google Fonts (Syne + DM Mono) | Typography |

---

## License

MIT
