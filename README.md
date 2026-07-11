# Glyph

A lightweight, distraction-free markdown editor with a live preview — built to run entirely in your browser, save your work automatically, and install like a native app on any device.

**Live app:** https://niranjanrath.github.io/Glyph/ *(update if your Pages URL differs)*

---

## Overview

Glyph is a single-page markdown editor with a split-view layout: write in plain markdown on one side and see it rendered instantly on the other. There's no backend, no account, and no sync server — everything is stored locally in your browser, so your notes stay private and available offline.

It's built mobile-first and scales up to tablet and desktop, with a clean, minimal interface that keeps the writing surface front and center.

---

## Features

- **Live split-pane preview** — write markdown on the left, see the rendered output on the right (desktop/tablet); a simple Edit / Preview toggle on mobile
- **Full markdown support** — headings, bold/italic, lists, blockquotes, links, images, code blocks, and GitHub-flavored tables
- **Auto-save** — every change is saved to your browser's local storage, with a subtle status indicator ("Saving…" / "Saved")
- **Manual actions** via the menu:
  - Save
  - Download as `.md`
  - Export the rendered note as `.pdf`
  - Print
  - Clear all content
- **Light / Dark theme** — remembers your preference for future visits
- **Installable (PWA)** — add Glyph to your phone's home screen or desktop for an app-like experience with offline support
- **No account, no server** — all data lives in your browser only

---

## Tech Stack

Built entirely with client-side web technologies — no build step, no framework, no backend:

- **HTML5** for structure
- **CSS3** for responsive, mobile-first styling and theming
- **Vanilla JavaScript (ES6+)** for editor logic, auto-save, and rendering
- **[marked.js](https://github.com/markedjs/marked)** for markdown parsing
- **[DOMPurify](https://github.com/cure53/DOMPurify)** for sanitizing rendered HTML
- **[jsPDF](https://github.com/parallax/jsPDF) + [html2canvas](https://github.com/niklasvh/html2canvas)** for PDF export
- **Service Worker + Web App Manifest** for offline support and installability

---

## Getting Started

### Use it online
Just open the [live app](https://niranjanrath.github.io/Glyph/) in any modern browser — nothing to install.

### Run it locally
```bash
git clone https://github.com/niranjanrath/Glyph.git
cd Glyph
python3 -m http.server
```
Then open `http://localhost:8000` in your browser.

> Note: the service worker and "Add to Home Screen" install prompt only work over `https://` or `localhost` — not when opening `index.html` directly as a local file.

### Install as an app
- **Android (Chrome):** open the site → tap the menu → **Add to Home screen**
- **iPhone (Safari):** open the site → tap **Share** → **Add to Home Screen**
- **Desktop (Chrome/Edge):** click the install icon in the address bar, or use the browser menu → **Install Glyph**

---


## Roadmap / Ideas

- Multiple notes with a sidebar or note list
- Full-text search across notes
- Keyboard shortcuts (bold, italic, headings)
- Synced scrolling between editor and preview
- Export to additional formats (HTML, DOCX)

---

## License

No license specified yet — add one (e.g. MIT) if you plan to open this up for others to use or contribute to.
