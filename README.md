# Evergreen Executive Portfolio Template

A JSON-driven portfolio website template. All content lives in `data/*.json` — edit those files to personalize the site. Built with vanilla HTML/CSS/JS, deployable on GitHub Pages.

## Editing and building

Content lives in `data/*.json` and the page template in `src/index.html`. The root `index.html` is generated so search engines and link previews see real content without running JavaScript.

```bash
npm install
npm run build   # writes index.html from src/index.html + data/*.json
```

A GitHub Action (`.github/workflows/prerender.yml`) also regenerates and commits `index.html` automatically whenever `src/`, `data/`, `scripts/` or `assets/js/main.js` change on `main`.
