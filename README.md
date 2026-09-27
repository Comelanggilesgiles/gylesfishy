# Gylesfishy

A hand-drawn, scroll-animated brand site for a specialty taiyaki shop.

## Description

Gylesfishy is a single-file, mobile-first landing page for a taiyaki (fish-shaped waffle) restaurant. It turns a plain business card into an interactive brand experience: the card tilts in 3D as you move your cursor, then melts into a scroll-locked sequence where a hand-drawn taiyaki swims into view, splits open, and its filling pops out into the menu categories. Every illustration — the fish, the steam, the filling grains — is inline SVG, drawn with a doubled, slightly offset outline to give it a hand-sketched feel. No frameworks, no build step, no dependencies beyond two Google Fonts.

## Key Features

- 3D hero card that tilts toward the cursor and expands into the brand reveal on scroll
- Scroll-locked "splitting taiyaki" sequence with bouncing filling grains that resolve into menu categories
- Horizontally scrolling product reel with tail-wag interaction on hover/tap
- Interactive filling selector that swaps cross-section color, background, price, and description on click
- Shop info section with a drop-bounce taiyaki and rising steam animation
- 100% inline SVG artwork, vanilla JavaScript, and CSS — a single portable HTML file

## Screenshot

![Gylesfishy homepage screenshot](/pic/fish.png)



## Tech Stack

- HTML5
- CSS3 (custom properties, keyframe animations, `IntersectionObserver`-driven reveals)
- Vanilla JavaScript (no frameworks or build tools)
- Inline SVG for all illustrations
- Google Fonts: Fredoka, Zen Maru Gothic

## Install & Usage

This is a static site — there is nothing to build or compile.

1. Clone the repository
   ```bash
   git clone https://github.com/Comelanggilesgiles/gylesfishy.git
   cd gylesfishy
   ```
2. Open it directly in a browser
   ```bash
   open index.html      # macOS
   start index.html      # Windows
   xdg-open index.html   # Linux
   ```
3. (Optional) Serve it locally instead of opening the file directly, so scroll behavior matches production
   ```bash
   npx serve .
   ```
   Then visit the local URL it prints (typically `http://localhost:3000`).

That's it — no dependencies to install.

## Deploying

Because it's a single `index.html` file, you can host it anywhere static files are served (GitHub Pages, Netlify, Vercel). For GitHub Pages: push to your repo, then enable Pages in **Settings → Pages** and point it at the `main` branch root.

## Committing Your Changes

```bash
git add .
git commit -m "Add Gylesfishy landing page"
git push origin main
```

If this is a brand-new repository, initialize it first:

```bash
git init
git remote add origin https://github.com/Comelanggilesgiles/gylesfishy.git
git branch -M main
git add .
git commit -m "Initial commit: Gylesfishy landing page"
git push -u origin main
```

## Notes

- Store details (address, phone, hours) in the Shop Info section are placeholders pulled from the brief — update them with your real business info before launch.
- Replace `screenshot.png` with an actual screenshot once the page is deployed.
