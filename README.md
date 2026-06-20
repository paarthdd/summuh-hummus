# Summuh Hummus — website

A single-page, scroll-driven site for **Summuh Hummus** (*Hummus, rewound.*).
One file, no build step, no dependencies — just open `index.html`.

## Preview locally
Double-click `index.html`, or run a tiny server:
```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Put it on GitHub Pages (free, ~2 min)

1. Create a new repo on GitHub, e.g. **`summuh-hummus`** (public).
2. Push this folder:
   ```bash
   git remote add origin https://github.com/<your-username>/summuh-hummus.git
   git branch -M main
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment → Source: `Deploy from a branch` → Branch: `main` / `root` → Save.**
4. Wait ~1 minute. Your site is live at:
   `https://<your-username>.github.io/summuh-hummus/`

> Tip: To use a custom domain like `summuhhummus.com`, add it under Settings → Pages → Custom domain, then point your domain's DNS at GitHub.

## Things you'll want to swap in
- **Founder photo** — the placeholder block in the *Founders* section. Drop in a real image: add the file (e.g. `founders.jpg`) and replace the `.ph` placeholder `<div>` with `<img src="founders.jpg" alt="Paarth and Advik" style="width:100%;height:100%;object-fit:cover">`.
- **Social links** — Instagram / TikTok `href="#"` in the footer.
- **Waitlist form** — wired for [Formspree](https://formspree.io). Create a free form, then paste your form ID into `const FORMSPREE_ID = ""` near the bottom of `index.html`. Signups will land in your Formspree inbox/dashboard. Until you add the ID, the form still shows a thank-you and logs the email to the console.
- **Stat numbers** — edit the `data-count` values in the *Stats* section if your lab-verified macros change.

## Edit the copy
Everything lives in `index.html` — section text is plain HTML, easy to find by the comment headers (`<!-- ============ STORY ============ -->`, etc.).
