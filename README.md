# 📅 Weekly Timetable

A clean, installable weekly timetable app for **B.Tech Integrated Data Science — Sem XI (Sections E1 & E2)**. Works offline, installs like a native app on Android and iPhone, and switches between a mobile-friendly day view and a full desktop grid view.

**🔗 Live app:** [aayushhn123.github.io/Weekly-Timetable](https://aayushhn123.github.io/Weekly-Timetable/)

---

## ✨ Features

- **📱 Day view (agenda)** — scrollable list of today's (or any selected day's) classes with time, subject, room, and faculty. Optimized for phones.
- **🖥️ Week view (grid)** — full Monday–Sunday timetable grid for wider screens, with sticky headers and time column.
- **🔀 Section toggle** — switch instantly between Section E1 and Section E2.
- **📆 Day navigator** — quick-jump pills to any day of the week (mobile view).
- **🟢 Today highlighting** — current day is auto-highlighted in both views, with a "TODAY" badge.
- **🎨 Color-coded lecture types:**
  - 🟢 Common lecture (shared across sections)
  - 🟠 Class-specific lecture
  - 🟤 Reserved for extra lecture
  - 🔴 Holiday
  - ⚪ Free / no lecture
  - ⬜ Break
- **👩‍🏫 Faculty & subject legend** — quick reference table of subject codes, full names, and faculty.
- **📲 Installable app (PWA)** — add it to your home screen on **Android** or **iPhone** and it behaves like a native app (its own icon, no browser address bar).
- **📡 Offline support** — once loaded, a service worker caches the app so it keeps working with no internet connection.
- **🌐 Install banner** — the app prompts you to install itself, with tailored instructions for iOS vs Android.

---

## 📥 How to install

### Android (Chrome)
1. Open the [live link](https://aayushhn123.github.io/Weekly-Timetable/)
2. Tap **Add to Home Screen** when the banner appears (or use Chrome's menu → *Install app*)

### iPhone (Safari)
1. Open the [live link](https://aayushhn123.github.io/Weekly-Timetable/) in **Safari** (not Chrome)
2. Tap the **Share** icon
3. Tap **Add to Home Screen**

> Once installed, the app opens full-screen with its own icon — just like a regular app.

---

## 🗂️ Repo structure

| File | Purpose |
|---|---|
| `index.html` | Main app — timetable data, layout, and all logic |
| `manifest.json` | PWA config (app name, icons, theme colors) |
| `sw.js` | Service worker — enables offline caching |
| `icon-192.png`, `icon-512.png` | App icons (Android) |
| `icon-512-maskable.png` | Adaptive icon (Android) |
| `apple-touch-icon.png` | Home screen icon (iOS) |
| `favicon-32.png`, `favicon-16.png` | Browser tab favicons |

---

## 🛠️ Updating the timetable

All schedule data lives inside `index.html` in the `DATA` and `WINDOWS` JavaScript objects near the bottom of the file. Edit the relevant day/section entry, commit, and GitHub Pages will redeploy automatically within a minute or two.

---

## 📌 Notes

- Hosted via **GitHub Pages** — HTTPS is required for offline/install features to work, so the app only behaves as a full PWA when accessed via the live link above (not when opened as a local file).
- w.e.f. 13 July 2026 · Rev 0
