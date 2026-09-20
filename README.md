# Value Connect Redesign

Redesign of the [Value Connect](https://valueconnectonline.co.ke) website.

This repository starts from a clean static template and will be progressively
redesigned to migrate Value Connect's content, branding, and services.

## Tech Stack

- Static HTML (single page: `index.html`)
- [Tailwind CSS v4](https://tailwindcss.com/) compiled with the Tailwind CLI
- [Alpine.js](https://alpinejs.dev/) via CDN (dark-mode toggle and small interactions)
- [Inter](https://fonts.bunny.net/) web font via bunny.net

The site itself is plain static HTML/CSS/JS. The only tooling is the Tailwind
CLI, used to compile `src/input.css` into `assets/css/style.css`. The compiled
CSS is committed, so the site runs without a build step.

## Getting Started

Open `index.html` directly in a browser, or serve the folder statically, e.g.:

```
python3 -m http.server
```

then visit http://localhost:8000.

## Building the CSS

Only needed when editing markup classes or `src/input.css`:

```
npm install        # first time only
npm run build      # compile once (minified)
npm run watch      # rebuild on change during development
```

## Project Structure

```
index.html         # Page markup
src/input.css      # Tailwind CSS source (directives, theme, dark-mode variant)
assets/css/        # Compiled stylesheet (style.css, generated)
assets/            # Images (photo + project thumbnails)
```

## Credits

Built on the "Olivia" portfolio template, © [Pixelcave](https://pixelcave.com/),
distributed by [ThemeWagon](https://themewagon.com/) under the MIT license.
