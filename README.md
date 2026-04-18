# Shikhar Shrestha — Portfolio Website

A multi-page, fully responsive portfolio site with a Netflix-inspired red & black theme.

---

## 📁 File Structure

```
portfolio/
├── index.html              ← Home page (hero + summary + impact)
├── experience.html         ← Professional Experience
├── education.html          ← Education + Certifications
├── projects.html           ← Class Projects (editable template)
│
├── css/
│   └── styles.css          ← All styles (shared across pages)
│
├── js/
│   └── main.js             ← Navigation + interactions
│
├── assets/
│   ├── profile.jpg         ← ADD your square profile photo here
│   ├── logos/              ← (optional) host your own company logos
│   └── projects/           ← ADD project screenshots/videos here
│
└── README.md
```

---

## 🚀 Deploy to GitHub Pages (Free Hosting)

1. Create a new repository on GitHub (e.g., `shikhar-portfolio` or `shikhars.github.io`).
2. Upload **everything inside this `portfolio/` folder** to the repository root — not the folder itself, just its contents.
3. In the repo: **Settings → Pages → Branch: main → / (root) → Save**.
4. Your portfolio will be live at:
   - `https://<username>.github.io/shikhar-portfolio/` (project repo), or
   - `https://<username>.github.io/` (if repo is named `<username>.github.io`).

---

## ✏️ Customization Checklist

### 1. Profile Photo (Home page)
Add a square profile photo:
- File: `assets/profile.jpg`
- Recommended: 500×500 px or larger, square aspect ratio
- If no photo is present, the page shows a stylized "SS" placeholder automatically.

### 2. LinkedIn URL (Home page)
Open `index.html` and find:
```html
<a href="#" target="_blank" rel="noopener" class="contact-item">
```
Replace `#` with your LinkedIn profile URL (e.g., `https://www.linkedin.com/in/shikharshrestha`).

### 3. Coursework (Education page)
Open `education.html`. The coursework lists include placeholder courses tied to your stated MBA concentration and IS undergrad. Replace each `<li>` with the specific courses you've taken.

### 4. Class Projects (Projects page)
Open `projects.html`. Each `<article class="project-card">` is a template. For each real project:
- Add your screenshot to `assets/projects/` (e.g., `project-1.png`)
- Update the `<img src="...">` path
- Edit the `<span class="project-tag">`, `<h3 class="project-title">`, `<p class="project-desc">`
- Update tech pills and buttons
- To embed a video, replace the `<img>` tag with:
  ```html
  <video src="assets/projects/your-demo.mp4" controls muted loop playsinline></video>
  ```
- Remove the yellow/red "Template Instructions" block once you've customized.

### 5. Company Logos (Experience page)
Company logos ship locally as SVGs at `assets/logos/*.svg` (Tyson, MACC, Creighton). They are original wordmark designs sized for the dark theme. To use a different logo, replace the file at that path — the HTML just points at it.

If an image fails to load, the company initials appear as a fallback.

---

## 🎨 Theme

- **Netflix Red** `#E50914`
- **Background Black** `#0a0a0a` / `#141414`
- **Typography:** Bebas Neue (display), Oswald (headings), DM Sans (body)
- Fully responsive: desktop, tablet, mobile (tested down to 320px)
- Mobile nav: hamburger menu
- Respects `prefers-reduced-motion`

---

## 📱 Screen Size Compatibility

| Device           | Status |
|------------------|--------|
| 4K / Large Desktop | ✅ |
| Laptop / Desktop   | ✅ |
| Tablet (portrait/landscape) | ✅ |
| Mobile (down to 320px) | ✅ |

---

## 🛠️ Local Preview

Just open `index.html` in any browser — no build step, no dependencies.

Or run a quick local server:
```bash
# Python
python3 -m http.server 8000
# then open http://localhost:8000
```

---

© Shikhar Shrestha · Fort Worth, Texas
