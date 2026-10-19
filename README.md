# Southery Menu — web page

A single page that shows the four Southery menu pages as SVG images, on Malabar green.

- `public/index.html` — the page
- `public/menu/page-1.svg` … `page-4.svg` — the menu pages (from `UPDATED TAKEAWAY MENU.pdf`)
- `vercel.json` — Vercel settings (serves `public/`, caches the menu images for a day)

No build step. Total size about 1.2 MB.

## Put it live on Vercel (free)

**Option A — no code (GitHub + Vercel website)**

1. On github.com, create a new repository named `southery-menu`.
2. Click **Add file → Upload files** and drag in the *contents* of this folder (`public`, `vercel.json`, `README.md`). Commit.
3. On vercel.com, click **Add New → Project**, pick `southery-menu`, leave every setting as it is, and click **Deploy**.
4. You get a link like `southery-menu.vercel.app`. Add your own domain later under **Settings → Domains**.

**Option B — from a laptop with Node.js**

```
cd southery-menu
npx vercel --prod
```

## Updating the menu later

Export the new menu from Illustrator as PDF, replace the SVGs in `public/menu/`, and push to GitHub. Vercel redeploys on its own.
