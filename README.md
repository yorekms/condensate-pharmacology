# Deploying Your GitHub Pages Research Hub & Password-Gated Preprint Portal

- **Public Link-Out Hub:** `docs/index.html` — Connects Paper #1, Paper #2 (linking to password-gated `preprints.html`), and your already-posted Seizure Transcriptomics & Epilepsy Bioinformatics portal.
- **Password-Gated Full Preprints & 3D Viewers:** `docs/preprints.html` — Passphrase: `matt said it was okay` (stored only as a SHA-256 hash).
- **Direct Zero-Login Review Link for Dr. Johannes W. Hell:** `docs/johannes-hell-brief-8f4b2c.html` (unlisted, `noindex, nofollow` + `robots.txt` disallowed; opens Paper #1 PDF, 2-Page Brief PDF, and all 3 interactive WebGL viewers with one click).

## Quick 3-Step Publish
1. Create a GitHub repository (e.g. `yorekms/condensate-pharmacology-preprints`).
2. Push this `docs/` folder to `main`:
   ```bash
   git init && git add docs && git commit -m "Publish research hub and password-gated preprint portal"
   git branch -M main && git remote add origin https://github.com/yorekms/condensate-pharmacology-preprints.git && git push -u origin main
   ```
3. In GitHub: **Settings → Pages → Source: Deploy from a branch → Branch: `main`, Folder: `/docs` → Save**.
   - Public Research Link-Out Hub: `https://yorekms.github.io/condensate-pharmacology-preprints/`
   - Password-Gated Preprints & 3D Viewers: `https://yorekms.github.io/condensate-pharmacology-preprints/preprints.html`
   - Johannes Hell's direct zero-login link: `https://yorekms.github.io/condensate-pharmacology-preprints/johannes-hell-brief-8f4b2c.html`
