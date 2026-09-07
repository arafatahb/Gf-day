# Happy Girlfriend Day 💌

A single-page, animated 3D web experience built for Girlfriend Day (Aug 1). No frameworks, no build step — just open it and go.

## What's inside
- **Hero** — full-screen intro with a real-time 3D floating heart field, built with three.js (particles react to your mouse).
- **Envelope** — a 3D CSS envelope you click to open, revealing a personal letter.
- **Stats** — a "days together" counter based on a date you set.
- **Flip cards** — 10 reasons, revealed with a 3D flip on tap.
- **Carousel** — a 3D coverflow gallery containing six included cute illustrated portraits.
- **Closing** — a heartbeat animation and a "Send Love" button that bursts floating hearts.
- **Project fullscreen** — a fixed button in the bottom-right corner opens the complete experience in browser fullscreen.

## How to run it
1. Unzip the folder.
2. Open the folder in VS Code.
3. Install the **Live Server** extension (if you don't have it), right-click `index.html` → **Open with Live Server**.
   - Or just double-click `index.html` to open it in your browser directly.
4. Click the **✎ Edit** button (top right) to set her name, your signature, and your "together since" date. It saves in the browser automatically.
5. Click **Full Screen** in the bottom-right corner for fullscreen mode. Press **Esc** to exit.

## Customizing
- **Name / signature / date**: use the ✎ Edit panel in the browser — no code needed.
- **The letter text**: edit the `<div class="letter">` paragraph content in `index.html` (around line 45).
- **The 10 reasons**: edit the `reasons` array near the top of `script.js`.
- **Gallery images**: six local portrait illustrations are already included in `assets/` and loaded from the `portraits` array inside `initCarousel()` in `script.js`.
- **Use your own photos later**: add your files to `assets/`, then replace any `src` value such as `assets/cute-girl-1.svg` with `assets/photo1.jpg`. Keep portrait photos around a 4:5 ratio for the cleanest result.
- **Colors**: all colors are CSS variables at the top of `style.css` under `:root` — change `--rose`, `--gold`, `--bg-deep`, etc.

## Notes
- Uses three.js r128 via CDN (`cdnjs.cloudflare.com`) and Google Fonts (Playfair Display + Quicksand) — an internet connection is needed the first time these load.
- Fully responsive, works on mobile.
- Respects `prefers-reduced-motion`.

Made for Girlfriend Day, Aug 1. 🤎
## Full-view gallery

- Click the active center portrait (or press Enter/Space) to open it in a full-screen viewer.
- Press **Esc**, click the **×** button, or click the dark backdrop to close it.
- Use the arrow keys/buttons or swipe on mobile to change photos while the viewer is open.

