# 🎨 ALPis Content Studio

A web-based content creation platform that helps users generate, adapt, and manage digital content for multiple channels from one interface.

🔗 **Live Demo:** https://laurandreea10.github.io/ALPis-CONTENT-STUDIO/

---

## 🚀 Overview

ALPis Content Studio is a centralized UI that groups content tools in one place:

- social captions
- hashtags
- ad text
- video scripts
- brand assets (flyers, banners, palettes)

The current build is intentionally front-end only and simulates an AI-assisted workflow.

---

## ✨ Features

- ✍️ Text adaptation for multiple platforms
- 🏷️ Caption & hashtag generation
- 📢 Bio & CTA generation
- 🖼️ Image tools & thumbnail controls
- 🎬 Video scripting assistant
- 📊 Marketing/ad generation blocks
- 🌍 Bilingual UI (RO / EN)
- 📱 Responsive sidebar layout

---

## 🧭 How it works

1. Pick a tool from the left navigation.
2. Fill in the short form inputs.
3. Generate output blocks (text/image/script).
4. Copy, regenerate, and iterate.

The app is organized as a modular single-page interface where each tool has its own render function and shared utility helpers.

---

## 🏗️ Architecture

This repository currently contains a single static entry point:

- `index.html` – structure, styles, i18n dictionary, UI components, and behavior.

Major architecture blocks inside `index.html`:

- global design tokens and CSS utilities
- navigation builder + view switcher
- per-tool render functions
- shared helpers (toast, copy, language switching)

---

## ♿ Accessibility improvements included

- `aria-label` for icon-only actions (including mobile menu)
- visible `:focus-visible` states for keyboard users
- skip link for direct main-content navigation
- semantic landmarks (`nav`, `main`) improved with labels/attributes
- keyboard enhancement: `Esc` closes the mobile sidebar

---

## 🔎 SEO & Share preview improvements included

- `meta description`
- Open Graph (`og:title`, `og:description`, `og:image`, `og:url`)
- Twitter card metadata
- `theme-color`
- inline SVG favicon
- simple `SoftwareApplication` JSON-LD schema

---

## 🖼️ Preview

> Replace the placeholders below with real captures from your deployed app.

- `docs/screenshots/dashboard.png`
- `docs/screenshots/ad-generator.png`
- `docs/screenshots/video-script.png`
- `docs/screenshots/image-tools.png`
- `docs/screenshots/mobile-sidebar.png`

For best first impression, also add:

- 1 short GIF with the main flow (`select tool -> generate -> copy`)

---

## ⚙️ Tech Stack

- HTML
- CSS
- JavaScript
- GitHub Pages

---

## ⚠️ Known limitations

- No backend persistence (state resets on reload)
- No real model/API integration by default
- Very large single-file architecture (harder long-term maintenance)
- Limited automated test coverage

---

## 🧪 Minimal test plan

- Smoke test top 5 tools (adapt, hashtag, caption, video, ads)
- Keyboard-only navigation test
- Mobile sidebar open/close + escape behavior
- Meta tags validation on deployed page
- Lighthouse pass target for Accessibility/SEO baseline

See full checklist in [`TEST_PLAN.md`](TEST_PLAN.md).

---

## 🗺️ Project maturity

This repo now includes:

- roadmap: [`ROADMAP.md`](ROADMAP.md)
- changelog: [`CHANGELOG.md`](CHANGELOG.md)
- issue template: [`.github/ISSUE_TEMPLATE/bug_report.md`](.github/ISSUE_TEMPLATE/bug_report.md)
- license: [`LICENSE`](LICENSE)

Recommended GitHub sidebar setup:

- **Description:** “AI-inspired content studio for multi-platform text, visual and video workflows.”
- **Topics:** `content-studio`, `social-media-tools`, `javascript`, `frontend`, `ai-workflow`, `productivity`, `single-page-app`

---

## 🎯 Purpose

The project explores how a modern content creation product could feel in-browser, with fast iteration and many utility flows in one place.
