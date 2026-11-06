# Portfolio — João Henrique

**Author:** João Henrique Porfirio Firmiano

Personal portfolio website with a scroll-driven animation: a 2D character falls backwards into the water, the water rises and covers the page, and the projects appear underwater.

## Features

- Scroll-driven character animation (13-frame sequence)
- Pixel-art water, bubbles, splash, trail and swimming sharks drawn on `<canvas>`
- EN / PT language toggle with a binary "decoding" text effect
- Project cards with screenshot galleries
- Plain HTML, CSS and JavaScript — no framework, no build step

## Structure

```
index.html        page, styles and scripts
img/f/            character animation frames
img/p/            project screenshots
img/              shark sprite and social icons
fonts/            self-hosted fonts (Silkscreen, Poppins, Space Grotesk)
```

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8080
```

## Deploy

Static site — import the repository in Vercel with the default settings (no build command, output directory `.`).
