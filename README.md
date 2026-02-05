# Cursor Landing Page Clone

A static HTML/CSS recreation of the Cursor home page as seen on 2026-02-05. Live demo: https://cursor-ai-vanila-version.netlify.app/

## Sections Recreated
- Header with logo, primary navigation, and auth/download buttons
- Hero block with main headline and primary CTA
- Brand trust row with partner logos grid
- Agent feature trio (Agent, Tab autocomplete, Ecosystem)
- Testimonial grid
- Frontier feature cards
- Changelog highlights
- Careers/advert banner strip
- Recent highlights sticky heading + cards
- Final CTA banner
- Footer with multi-column links and legal strip

## Fonts & Colors
- Font: `Carrois Gothic` via Google Fonts; fallbacks: system-ui, Helvetica Neue, Helvetica, Arial, sans-serif (body) and system defaults for paragraphs.
- Core palette (CSS variables in `src/style.css`):
  - `--bg-color`: #14120b (page background)
  - `--primary-text`: #ffffff
  - `--secondary`: #cccccc
  - `--teritary`: #1d1b15 (card backgrounds)
  - `--acent`: #f54e00 (links/CTAs)
- Card hover and section-specific colors follow the same palette (e.g., recent highlights cards use #22201b / #26241e on hover).

## File Structure
- `index.html` — page markup
- `src/style.css` — global styles and layout grid definitions
- `public/images` — assets (logos, hero banner, feature art, testimonials, frontier images, changelog, etc.)

## Running Locally
1) Install deps (Vite only): `npm install`
2) Start dev server: `npm run dev`
3) Open the printed localhost URL.

## Screenshots (add yours)
Place exported screenshots in `public/screenshots/` and reference them below:
- `public/screenshots/hero.png`
- `public/screenshots/full-page.png`

```
![Hero](public/screenshots/hero.png)
![Full page](public/screenshots/full-page.png)
```

## Publishing to a Public GitHub Repo
1) Initialize git: `git init`
2) Add files: `git add .`
3) Commit: `git commit -m "Add Cursor clone"`
4) Create a new public repo on GitHub (UI or `gh repo create --public cursor-clone`)
5) Connect remote: `git remote add origin <your-repo-url>`
6) Push: `git push -u origin main`

## Known Notes
- The "Recent highlights" heading uses `position: sticky` at `top: 10%`; ensure the parent has no `overflow` that would disable stickiness and that content is tall enough to scroll.
- Icons/arrows currently use text arrows; swap for SVGs if desired.

## Live Demo
- Netlify: https://cursor-ai-vanila-version.netlify.app/
