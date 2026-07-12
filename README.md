# Developer Portfolio — TaskFlow Task 1

A three-page, responsive static portfolio site built as Task 1 of the TaskFlow
internship project (Environment Setup & Static Website Deployment).

## Live site

_Add your live URL here after deploying, e.g._
`https://yourusername.github.io/portfolio-site/` or `https://your-portfolio.netlify.app`

## Pages

- `index.html` — Home: intro, project grid, skills panel
- `about.html` — About: bio + a build log mapping all 6 TaskFlow tasks
- `contact.html` — Contact: form + direct contact details

## Structure

```
portfolio-site/
├── index.html
├── about.html
├── contact.html
├── styles/
│   └── main.css
├── scripts/
│   └── nav.js
├── images/
└── README.md
```

## Design

A "blueprint" visual system: deep blue background with a technical drafting
grid, an amber accent, monospace labels (JetBrains Mono) for structure, and
Space Grotesk for display type. The homepage hero is styled as a blueprint
title block with corner marks and a stamp/metadata row, echoing the idea of
this site being the first "build" in the TaskFlow project.

## Responsive behavior

- **Desktop (>768px):** horizontal nav, multi-column project/skill grids,
  two-column contact layout.
- **Mobile (≤768px):** nav collapses behind a hamburger button
  (`scripts/nav.js` toggles it), grids stack to a single column.

Test it in Chrome DevTools → Device Toolbar, or just resize the browser
window.

## Setup

No build step or dependencies. Open `index.html` directly in a browser, or
serve it locally:

```bash
# Using VS Code Live Server extension, or:
npx serve .
```

## Deployment

**GitHub Pages**
```bash
git init
git add .
git commit -m "Initial portfolio"
git remote add origin https://github.com/<username>/<repo-name>.git
git push -u origin main
```
Then: repo **Settings → Pages → Branch: main → Folder: / (root)**.

**Netlify**
Drag and drop this folder onto [Netlify Drop](https://app.netlify.com/drop),
or connect the GitHub repo through the Netlify UI.

## Design choices

- Semantic HTML5 (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`,
  `<footer>`) throughout.
- CSS Grid for the project/skill card layouts; Flexbox for nav and buttons.
- One shared stylesheet (`styles/main.css`) and one shared script
  (`scripts/nav.js`) across all three pages for consistency.
- Placeholder copy (name, email, project links) is marked for you to swap in
  your own details before submitting/deploying.

## Next steps (later tasks)

This repo is scoped to Task 1 only. Tasks 2–6 (TaskFlow frontend, backend,
database, auth, and deployment) build on top of this as separate,
progressively more complex deliverables.
