# Portfolio — João Henrique

**Author:** João Henrique Porfirio Firmiano

Personal portfolio website with a scroll-driven animation: a 2D character falls backwards into the water, the water rises and covers the page, and the projects appear underwater.

## Problem

My university projects were spread across separate repositories, and I had no single place to show them to recruiters and professors in a way that people would remember.

## Solution

I came up with the concept (my 2D character falling backwards into the water while the page scrolls) and used **Claude (Anthropic)** as a coding assistant to turn it into a working page: the scroll-synced 13-frame animation, the pixel-art water, bubbles and sharks drawn on `<canvas>`, the EN/PT toggle and the project cards. I reviewed each version in the browser and asked for adjustments until it matched the idea. Claude also helped me deploy it to Vercel and add Vercel Web Analytics.

## Technologies

- HTML, CSS and JavaScript (Canvas API), with no framework and no build step
- Claude (Anthropic): AI coding assistant
- Vercel: hosting and Web Analytics

## Demo

Live site: **https://joaohpf.dev/**

## Result

- One link that presents all my projects, with screenshots, in English and Portuguese.
- Effects that would have taken me a long time to code alone (canvas animation synced to the scroll) were built and refined in a few rounds of feedback.
- Visits are measured with Vercel Web Analytics.

## Repository

- **Code:** the whole site is in `index.html`; images and fonts are in `img/` and `fonts/` (see [Structure](#structure)).
- **Run:** see [Run locally](#run-locally) and [Deploy](#deploy).

```bash
git clone https://github.com/joaohpf/MyRepository.git
cd MyRepository
python3 -m http.server 8080
```

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
