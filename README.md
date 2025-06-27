# task-web-application
# 🗂️ Task Web Application

A lightweight, single-page **task manager** that runs 100 % in the browser.  
Create, edit, search and delete tasks—everything is saved to **Local Storage**, so your list survives a page refresh without any back-end at all. Perfect for quick personal use, tutorials or hack-days.

<div align="center">
  <!-- Replace with real screenshots if available -->
  <img src="docs/demo.gif" width="700" alt="Tasky demo gif">
</div>

---

## ✨ Features

| Core | UX niceties |
|------|-------------|
| **Add tasks** with title, description, type & optional cover image | Modal-style *“Add New Task”* form |
| **Instant search** – filter cards as you type | Responsive layout & a fixed “+ Add” bar on mobile |
| **Inline edit & save** – click **Edit**, change text in-place, then **Save** | Tiny footprint—pure HTML + CSS + vanilla JS |
| **Delete** single cards | No build-step, deploy on any static host in seconds |
| **Open Task** modal shows full details & creation date | Data stored in `localStorage` so nothing is lost |

_Source peek » the whole flow lives in_ `index.js` :contentReference[oaicite:0]{index=0}

---

## 🔧 Tech Stack

| Layer | What we use |
|-------|-------------|
| Mark-up | `index.html` (plain HTML + embedded [Bootstrap 5] classes for ready-made grid, buttons & modals) |
| Styling | `style.css` / `index.css` for a minimal, soft-blue theme |
| Logic | **Vanilla JavaScript** (~51 % of repo lines) :contentReference[oaicite:1]{index=1} |
| Storage | Browser **LocalStorage**—zero server code required |

> **Why no frameworks?**  
> The repo keeps dependencies to zero so you can drop it anywhere—GitHub Pages, Netlify, Vercel, S3, even inside an Electron wrapper.

---

## 🚀 Getting Started

```bash
# 1 · Clone
git clone https://github.com/Surajgholase/task-web-application.git
cd task-web-application

# 2 · Just open the file
#    (or serve with Live Server / http-server for hot-reload convenience)
open index.html
# or
npx http-server .
