# Domain-Driven Portfolio

A multi-page static site built with HTML and CSS only. No frameworks. No JavaScript. No build tools. Deliberately minimal.

---

## The Thesis

**Learning to code doesn't require a toy project.**

Real domain work is enough. This portfolio is built around three domains — Networking, Data, and SWE — each of which generates real coding opportunities. The CCNA readiness report is the first module: an enterprise homelab assessment that became the vehicle for learning HTML and CSS.

The code is not decoration. The domain work is not a theme. They're the same thing.

---

## Project Structure

```
domain-driven-portfolio/
│
├── index.html      ← The hub — three domains, one page
├── ccna.html       ← CCNA 200-301 lab readiness report (Module 1 — Live)
├── data.html       ← Data module placeholder (Python · SQL · Pipelines)
├── swe.html        ← SWE module placeholder (Systems · APIs · Architecture)
│
├── css/
│   └── style.css   ← Shared stylesheet — every page links to this file
│
└── README.md       ← This file
```

---

## How to Read This Project

This project is designed to be read **twice** — once as a user, once as a developer.

**As a user:** Open `index.html` in a browser. Navigate to the CCNA report. Read the assessment.

**As a developer:** Open `ccna.html` and `css/style.css` in a code editor. Every element has a `<!-- 📘 -->` HTML comment. Every CSS rule has a `/* 📘 */` comment. The comments explain:
- What the element or rule is
- Why it was chosen over alternatives
- What concept it demonstrates
- A link to the W3Schools reference page

The source code is both a working page and a learning resource.

---

## Concepts Covered in the Code

| Concept | Where to see it |
|---|---|
| HTML document structure | Top of any `.html` file |
| Semantic HTML5 elements | `<nav>`, `<header>`, `<section>` in `index.html` |
| External stylesheet linking | `<link>` tag in every `<head>` |
| CSS custom properties (variables) | `:root` block in `style.css` |
| CSS Flexbox | `.verdict-box`, `.domain-header`, `.hub-card` in `style.css` |
| CSS Grid | `.row` and `@media` in `style.css` |
| Responsive design (media queries) | `@media (max-width: 500px)` in `style.css` |
| CSS pseudo-elements (::before) | `.item-good`, `.item-gap`, `.item-miss` in `style.css` |
| CSS pseudo-classes (:hover) | `.hub-link:hover`, `.nav a:hover` in `style.css` |
| Base + modifier class pattern | `.tag.tag-hard`, `.hub-card.active` in HTML files |
| Inline styles vs. class styles | Progress bars in `ccna.html` |
| HTML entities | `&amp;` in Domain 6 heading in `ccna.html` |
| Relative file paths | `href="ccna.html"`, `href="css/style.css"` |
| CSS specificity | Inline style overrides in `index.html`, `data.html`, `swe.html` |

---

## Stack

- **HTML5** — structure and content
- **CSS3** — layout (Flexbox, Grid), custom properties, responsive design
- **Google Fonts** — Syne + JetBrains Mono (loaded via `@import`)
- **No JavaScript** — every feature is CSS-only, intentionally
- **Deployed on Netlify** — static folder deploy, no build step required

---

## Living Document

The CCNA module (`ccna.html`) updates as real lab gaps are closed. Progress is tracked by exam domain. When a gap is addressed in the homelab, the domain score, progress bar, and item list update to reflect it. The commit history is the learning log.

**Current readiness: 74%**
Critical gaps: OSPFv2, IPv6, REST/Ansible automation (Domain 6)

---

## Author

WGU SWE student. Building across Networking · Data · SWE.
