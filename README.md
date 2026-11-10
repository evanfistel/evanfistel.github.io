# Evan Fistel — Portfolio

Plain HTML/CSS site hosted on GitHub Pages. No build step, no frameworks.

## Folder layout

```
index.html                  ← home: hero, projects, experience, skills, about
projects/_template.html     ← copy this for every new project write-up
projects/*.html             ← one page per project
assets/css/style.css        ← all styling (colors are at the top in :root)
assets/img/                 ← headshot.jpg + project images
assets/Evan_Fistel_Resume.pdf
```

## Put it online (one-time, ~10 minutes)

1. Create a GitHub account if you don't have one. Your username becomes the default URL, so pick something professional.
2. Create a new **public** repository named exactly `YOUR-USERNAME.github.io`.
3. Upload everything in this folder (drag and drop on the repo page works, or use GitHub Desktop).
4. Go to the repo's **Settings → Pages**, set Source to *Deploy from a branch*, branch `main`, folder `/ (root)`.
5. After a minute or two the site is live at `https://YOUR-USERNAME.github.io`.

## Before you publish — checklist

- [x] GitHub username filled in (evanfistel)
- [ ] Add `assets/img/headshot.jpg` (square crop works best)
- [ ] Add your resume as `assets/Evan_Fistel_Resume.pdf`
- [ ] Fill in the `<!-- TODO -->` comments in index.html (Experience bullets)
- [ ] Delete project cards you haven't built yet — empty placeholders look worse than fewer projects
- [ ] Nothing proprietary from Mercedes, LANL, Crimson Racing, or EcoCar without permission

## Custom domain (optional, ~$12/yr)

Buy `evanfistel.com` (or similar) from Cloudflare, Porkbun, or Namecheap, then in **Settings → Pages → Custom domain** enter it and follow GitHub's DNS instructions. Tick **Enforce HTTPS**.

## Adding a project

1. Copy `projects/_template.html` → `projects/your-project.html` and fill it in.
2. Export images as PNG/JPG under ~500 KB each into `assets/img/`.
3. On `index.html`, copy an existing `<a class="card">` block and point it at the new page.
4. For code projects (MATLAB, Python/FastF1), keep the code in its own repo and link it from the page's "Code / files" field.

## Preview locally

Open `index.html` in a browser, or run `python -m http.server` in this folder and go to http://localhost:8000.
