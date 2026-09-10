# AgriConnect — Smart Farming Platform

A landing page + working prototype (photo-based crop diagnosis, live weather,
voice alerts, simulated irrigation sensors) built with React, Vite, and
Tailwind CSS.

## Run it locally

```bash
npm install
npm run dev
```

Then open the local URL it prints (usually http://localhost:5173).

## Deploy it for free (pick one)

### Option A — Vercel (easiest)
1. Push this folder to a GitHub repo.
2. Go to vercel.com → "Add New Project" → import the repo.
3. Vercel auto-detects Vite. Click Deploy. Done — you get a live URL.

### Option B — Netlify
1. Push to GitHub.
2. Go to netlify.com → "Add new site" → "Import an existing project".
3. Build command: `npm run build`  |  Publish directory: `dist`
4. Deploy.

### Option C — GitHub Pages
```bash
npm run build
npm install -D gh-pages
```
Add to `package.json` scripts: `"deploy": "gh-pages -d dist"`
Then:
```bash
npm run deploy
```
Your site will be live at `https://<username>.github.io/<repo-name>/`

## Notes
- Weather uses the free Open-Meteo API (no API key needed).
- Voice output uses the browser's built-in Text-to-Speech — works best in
  Chrome. Tamil/Hindi voice availability depends on the visitor's device.
- Soil moisture / water tank level are simulated sliders standing in for
  real ESP32 sensors — swap these for live sensor data once hardware is wired in.
