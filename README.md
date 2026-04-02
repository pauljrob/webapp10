# webapp10 — Paul Roberts Portfolio

A single-page personal portfolio site for Paul Roberts, showcasing GitHub projects. Built with static HTML, CSS, and vanilla JavaScript — no build tooling required.

**Live site:** https://pauljrob.github.io/webapp10

---

## Local Development

No server required. Open the file directly in your browser:

```bash
open index.html         # macOS
start index.html        # Windows
xdg-open index.html     # Linux
```

All assets (fonts) load from Google Fonts CDN. An internet connection is required to load custom fonts; the site degrades gracefully to system fonts offline.

---

## Deployment (GitHub Pages)

1. Push your changes to the `main` branch.
2. Go to **Settings → Pages** in the repository.
3. Under **Source**, select **Deploy from a branch**.
4. Set the branch to `main` and the folder to `/ (root)`.
5. Click **Save**.

GitHub Pages will publish the site at `https://pauljrob.github.io/webapp10` within 1–2 minutes.

---

## Customization

All content is in `index.html`. Key locations:

| What to change | Where to find it |
|---|---|
| Name and tagline | `<h1 class="hero__name">` and `<p class="hero__tagline">` in the Hero section |
| Bio blurb | `<p class="hero__bio">` in the Hero section |
| Project cards (name, description, language, link) | Six `<article class="project-card">` blocks in the Projects section |
| About text | Two `<p class="about-block__body">` paragraphs in the About section |
| GitHub profile URL | `href="https://github.com/pauljrob"` (appears in nav and footer) |
| Color scheme | CSS custom properties in `:root {}` at the top of the `<style>` block |

---

## Tech Stack

- **HTML5** — semantic markup (`<header>`, `<main>`, `<section>`, `<footer>`, `<nav>`, `<article>`)
- **CSS3** — Custom Properties, CSS Grid, Flexbox, `clamp()`, `@keyframes`
- **Vanilla JS** — IntersectionObserver API for scroll-triggered card animations (~15 lines)
- **Google Fonts** — Cormorant Garamond, Syne, JetBrains Mono, Inter

No npm, no build step, no dependencies.
