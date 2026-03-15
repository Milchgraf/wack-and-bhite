# Schwellwert · Threshold Binarizer

A browser-based image tool that converts photos into two-color images using an adjustable luminance threshold. 100% vibe coded. ✨

## Features

- **Threshold conversion** – no grayscale, just a hard cut between dark and light based on luminance
- **Softness slider** – optional transition zone with a smoothstep curve
- **Custom colors** – pick any two colors instead of black and white
- **7 color presets** – B/W, Sepia, Cyanotype, Green, Red/Yellow, Night and more
- **Live histogram** – shows pixel distribution with threshold and softness markers
- **Fullscreen mode** – distraction-free view with zoom (scroll / `+`/`-`), pan (drag), fading HUD and full keyboard control
- **i18n** – German and English UI, auto-detected from browser language, togglable via DE / EN button
- **Drag & Drop** – just drop an image into the window
- **PNG export** – save the result directly

## Keyboard Shortcuts (Fullscreen)

| Key | Action |
|---|---|
| `F` | Open / close fullscreen |
| `← →` | Threshold ±1 |
| `↑ ↓` | Threshold ±10 |
| `Shift + ← →` | Softness ±1 |
| `Shift + ↑ ↓` | Softness ±10 |
| `+` / `-` | Zoom in / out |
| `0` | Reset zoom |
| `ESC` | Exit fullscreen |

**Zoom & Pan:** Scroll to zoom (centered on cursor), click & drag to pan.

## Usage

Just open `index.html` in a browser — no build step, no dependencies, no server required.

Or live on GitHub Pages: `https://milchgraf.github.io/wack-and-bhite/`

## Tech Stack

- [Vue 3](https://vuejs.org/) (via CDN, no build tooling)
- Vanilla Canvas API for image processing
- Perceptual luminance via BT.601 (`0.299·R + 0.587·G + 0.114·B`)
- Single HTML file

## License

MIT — do whatever you want with it.
