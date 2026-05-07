# Wakeboard101

A wakeboarding guide website built with pure HTML, CSS, and vanilla JavaScript. No frameworks, no build step — just drop the files on any static host or open them locally.

## Pages

| File | Description |
|------|-------------|
| `index.html` | Home / hero page |
| `beginner.html` | Beginner Skills module (stance, deep-water starts, edge control) |
| `tricks.html` | Trick Progression system (surface tricks → wake jumps → inverts) |
| `contact.html` | Contact form |
| `style.css` | All styles (CSS variables, responsive layout) |
| `script.js` | Mobile nav toggle + scroll-triggered animations |

## Running Locally

No server required — just open `index.html` in your browser:

```bash
open index.html
# or double-click index.html in Finder / Explorer
```

Or serve with any static server:

```bash
npx serve .
# or
python3 -m http.server 8080
```

## Deploying

Works with any static host:
- **GitHub Pages**: push to a repo and enable Pages on the `main` branch root
- **Netlify / Vercel**: drag-and-drop the folder
- **Cloudflare Pages**: connect your repo

## Design

- **Fonts**: Barlow Condensed (display) + Barlow (body) — Google Fonts
- **Colors**: `#1a6bff` blue accent, `#0a0a0a` near-black, white backgrounds
- **Hero images**: Unsplash (wakeboarding/water sports)
- **Layout**: CSS Grid, fully responsive down to 375px

## Customization

All colors and fonts are defined as CSS variables at the top of `style.css`:

```css
:root {
  --blue: #1a6bff;
  --black: #0a0a0a;
  --font-display: 'Barlow Condensed', sans-serif;
  --font-body: 'Barlow', sans-serif;
}
```

To replace hero images with your own photos, swap the `src` attributes in the `<img>` tags inside `index.html`.
