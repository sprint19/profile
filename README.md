# Sprint19 — Company Profile (one-pager)

A self-contained, single-file company profile for quick launch while the main
website revamp is in progress. No build step, no dependencies.

```
company-profile/
├── index.html        # the whole page (inline CSS)
├── assets/           # logos, headshots, OG image
└── README.md
```

## Deploy to GitHub Pages

1. Create a new GitHub repo (e.g. `sprint19/company-profile`).
2. Push this folder's contents to the repo's default branch:
   ```bash
   git init && git add . && git commit -m "Sprint19 company profile"
   git branch -M main
   git remote add origin https://github.com/sprint19/company-profile.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   then pick **`main` / `(root)`** and save.
4. The site goes live at `https://sprint19.github.io/company-profile/` within a minute.

### Custom domain (optional)
Add a `CNAME` file containing your domain (e.g. `profile.sprint19.com`) and point a
DNS CNAME record at `sprint19.github.io`. Set it under Settings → Pages → Custom domain.

## Editing
Everything lives in `index.html` — copy, colors (CSS variables in `:root`), services,
the process flow, the three featured-client quotes, leadership, and contact details.
Swap images in `assets/` keeping the same filenames.

## Notes
- Content and branding are reused from the main site (sprint19.com).
- Testimonials are from the PhilSME 2026 featured-client carousel.
