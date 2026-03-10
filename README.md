# Fractal Cycler (Website)

A fast, interactive fractal viewer built with **HTML Canvas + JavaScript + a Web Worker** so UI controls stay responsive while rendering.

## Features
- Fractal types: **Mandelbrot**, **Julia**, **Burning Ship**, **Tricorn**
- Live controls: iterations, zoom, center, Julia constant, color scheme
- Preset cycling (Prev/Next)
- Mouse controls:
  - **Drag** to pan
  - **Mouse wheel** to zoom (zooms around cursor)
- Worker-based rendering (prevents the page from freezing)
- Render token system (old renders are ignored when you change sliders quickly)

## Files
- `index.html` — UI + canvas + event handling
- `worker.js` — fractal computation in a Web Worker

## Run locally
Web Workers typically won’t work if you open `index.html` by double-clicking it. Use a local server:

```bash
python -m http.server 8000
