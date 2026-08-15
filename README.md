# ⚒️ BLOCKSMITH

### DRAG · DROP · SHIP

**Blocksmith** is a zero-dependency, **single-file drag & drop HTML studio**.
Compose landing pages, portfolios and full multi-page sites from ready-made blocks,
style them with themes & fonts, preview them live, and export clean standalone HTML —
**no build step, no framework, no server.** Everything runs in one HTML file, entirely client-side.

<!-- Optional: replace with a real screenshot -->
<!-- ![Blocksmith screenshot](docs/screenshot.png) -->

---

## ✨ Features

### 🧱 Builder
- **17 drag & drop blocks** — structure, text, media and engagement
- **Inline editing** — click any text and just type
- **Images** — browse for a file or drop image files straight onto the canvas
- **Hero, three ways** — solid color (incl. custom color picker), full-bleed **image**, or auto-playing **carousel** (up to 5 slides)
- **Hover toolbar** per block — drag-reorder, move up/down, duplicate, delete
- **Inspector** — per-block controls (levels, alignment, sizes, variants, padding, plans, slides, questions…)

### 📄 Pages & Site
- **Multi-page** projects with a video-editor style **timeline filmstrip** (live thumbnails, drag to reorder, rename, duplicate, delete)
- **Navigation manager** — toggle pages in/out of the menu; navbars & footers auto-generate real links
- **10 premade site themes** — one click applies colors, backgrounds and a matching font pairing
- **Font studio** — 19 Google Fonts + 10 system stacks, separate heading/body pairing
- **20 one-click web templates** — landing, product, portfolio, blog, SaaS, pricing, event, docs, restaurant, and more

### 📤 Output
- **Preview modal** with pixel-faithful render + **open in new tab**
- **HTML source view** with copy-to-clipboard
- **Export** a page or **all pages** as clean standalone `.html`
- **Open / Save project** as `.json` + automatic **localStorage autosave**
- **Undo / redo** history across the whole site
- **Light / dark studio mode** (persisted)
- **Device widths** — Desktop 960 · Tablet 768 · Mobile 390

---

## 🚀 Getting Started

1. Download / clone this repo.
2. Open `blocksmith.html` in any modern browser. *(That's the whole install.)*
3. Drag blocks from the left rail onto the canvas, click text to edit.
4. Style it in **SITE / THEMES**, or drop in a **TEMPLATE**.
5. Hit **EXPORT** (or `⌘S`) to download clean HTML.

---

## 🗺️ UI Overview

```
┌────────────────────────────────────────────────────────────────────┐
│ ◐ mode │ ⚒ BLOCKSMITH │  DESKOP/TABLET/MOBILE  │ NEW OPEN SAVE │ ↺ ↻ │ PREVIEW HTML │ EXPORT │
├──────────────┬──────────────────────────────────────┬──────────────┤
│ BLOCKS       │                                      │ INSPECTOR    │
│  palette     │            CANVAS (960px)            │  / SITE      │
│  (drag or    │     drop blocks · click to edit      │  / THEMES    │
│   click)     │                                      │  / TEMPLATES │
├──────────────┴──────────────────────────────────────┴──────────────┤
│ ▸▸ TIMELINE — page thumbnails · + page · dup · del · drag reorder  │
├────────────────────────────────────────────────────────────────────┤
│ ● AUTOSAVED · PAGE · n BLOCKS · THEME · shortcuts                  │
└────────────────────────────────────────────────────────────────────┘
```

---

## 🧱 Blocks (17)

| Group | Blocks |
|---|---|
| **Structure** | Navbar · Hero (color / image / carousel) · Columns · Footer |
| **Text** | Heading · Paragraph · Quote · List · Button · Code |
| **Media & Space** | Image · Divider · Spacer |
| **Engage** | Pricing Table · FAQ · Contact Form · Social Links (X / Instagram / Facebook / TikTok + more) |

## 🎨 Themes (10)

`FORGE` · `IVORY` · `CARBON` · `OCEAN` · `MEADOW` · `RUBY` · `MIDNIGHT` · `SUNSET` · `GLACIER` · `PAPERCUT`

## 📐 Templates (20)

Landing Page · Product Page · Portfolio · Blog Post · SaaS Startup · Pricing Page · Event Page · Docs Page · Restaurant · About/Team · Magazine · App Launch · Photo Gallery · Agency · Podcast · Résumé/CV · Coming Soon · Nonprofit · Property Listing · Newsletter

---

## ⌨️ Keyboard Shortcuts

| Keys | Action |
|---|---|
| `⌘Z` / `Ctrl+Z` | Undo |
| `⌘⇧Z` / `Ctrl+Y` | Redo |
| `⌘D` | Duplicate selected block |
| `DEL` / `Backspace` | Delete selected block |
| `⌥↑` / `⌥↓` | Move selected block up / down |
| `⌘S` | Export current page (`.html`) |
| `⌘⇧S` | Save project (`.json`) |
| `⌘O` | Open project (`.json`) |
| `ESC` | Close overlay / deselect |

---

## 🗂️ Project Save Format

Projects serialize to a single JSON document (also autosaved to `localStorage`):

```json
{
  "app": "blocksmith",
  "version": 2,
  "site": { "theme": "forge", "fonts": { "heading": "Space Grotesk", "body": "Space Grotesk" } },
  "pages": [ { "id": "…", "name": "Home", "bg": "#ffffff", "inNav": true, "blocks": [ … ] } ]
}
```

---

## 🛠️ Under the Hood

- **One HTML file**, vanilla JS — no dependencies, no build tooling.
- A **shared render stylesheet** powers the canvas, timeline thumbnails, preview and exported files, so what you see is exactly what ships.
- Simple **state → render** pipeline with snapshot-based **undo/redo**.
- Exported pages are self-contained (inline CSS + optional Google Fonts link) and host anywhere.

## 🌐 Browser Support

Latest Chrome, Edge, Firefox and Safari. Uses modern APIs (`contenteditable`, HTML5 drag & drop, `<details>`, CSS custom properties).

## 🛣️ Roadmap

- [ ] Touch / pointer-based drag & drop
- [ ] More column layouts & grid blocks
- [ ] Custom theme editor (save your own themes)
- [ ] Import exported pages back into the studio

## 📜 License

MIT — free to use, modify and ship. *(Replace with your license of choice.)*

---

> Built by hand with Blocksmith, naturally. ⚒️
