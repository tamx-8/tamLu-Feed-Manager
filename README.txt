tamLu Feed Manager v0.2
========================

Contents
- index.html: web app
- manifest.json: installable web app metadata
- sw.js: basic offline cache support

Try locally
1. Extract the ZIP.
2. Open index.html in a modern browser.

Publish online
Upload the extracted folder contents to a static hosting service that supports HTTPS
(for example, GitHub Pages, Netlify, or Cloudflare Pages). Upload the files themselves,
not just the ZIP, unless the hosting service explicitly accepts ZIP deployment.

Features
- Four herd groups
- Shared per-head feed amount
- Per-group herd and feeding head counts
- Auto-calculated kilograms and ratio gauges
- Gauge color: blue <= 90%, green > 90% and < 110%, red >= 110%
- Gauge scale 0–130%, with 100% marker
- Per-round task checklist
- Automatically saves settings and checklist in this browser using localStorage
- Removed the sample-value reset button

Prototype limitations
- No accounts or employee-to-employee cloud sync yet.
- Saved data stays in this browser on this device; it does not sync between employees or devices. Clearing browser data may erase it.
- Sample numbers are demo values; verify all amounts before operational use.
