# EOEX Academy

A responsive, zero-dependency single-page Academy catalogue. Open `index.html` directly or serve this folder with any static web server.

## Experience

- Six catalogue shelves with editorial cover cards that reveal a synopsis when turned.
- Twelve cards per view; Classes, Courses, Private Tuition and The Library have next/previous pagination.
- Muted looping video previews load only while their cards are near the viewport. Poster photography remains visible before playback and if a clip cannot load.
- The registration enquiry is a separate in-app view. A selected pathway and card are carried through from an enquiry button.
- French is the first-visit language. A compact, mobile-friendly selector switches the interface and full catalogue to English, Spanish, Italian, Portuguese or German; a saved preference is restored on return.
- The footer links to EOEX Agency, CARTESIENES and EOEX Publishing.
- GitHub Actions deploys the static site to GitHub Pages on pushes to `main`.

## Deployment

GitHub Pages must be enabled with **GitHub Actions** as its build and deployment source in the repository's Pages settings. Once enabled, the workflow in `.github/workflows/deploy-pages.yml` publishes the site after each push to `main` or a manual workflow run.

## Content and media

Showcase, Masterclass, Private Tuition and Library entries are defined in the inline script in `index.html`. The complete supplied 400-lesson and 53-pathway Course catalogues are in `catalogue-data.js`. The bundled translations are in `locale-data.js`. Cover photography is served by Unsplash and the sample fashion footage by Pexels; an internet connection is needed for remote media. Replace the sample footage and poster URLs with Academy-owned assets before production.

The registration form is a front-end preview only. It validates the fields in the browser, but does not send or store personal information. Connect it to an approved registration service before accepting real enquiries.
