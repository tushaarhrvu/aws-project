# ShopAll — How to Put It Online (Free)

Your site is a single file (`index.html`) with no server or database, so it can go live in minutes on any free static host. Pick ONE option below.

---

## Option 1 — Netlify Drop (easiest, ~2 minutes, no account signup needed to start)

1. Open your browser and go to: **https://app.netlify.com/drop**
2. Open File Explorer to `C:\Users\tusha\Downloads\AWS\`
3. Drag the **whole AWS folder** onto the Netlify Drop page.
4. Wait ~20 seconds. Netlify gives you a live URL like `https://random-name-123.netlify.app`
5. Share that URL — it works in any browser, on any device, anywhere.

To get a nicer name (e.g. `shopall.netlify.app`) or update the site later, create a free Netlify account when prompted.

---

## Option 2 — GitHub Pages (best if you want a permanent home + version history)

1. Create a free account at https://github.com
2. Create a new **public** repository named `shopall` (or anything).
3. Upload `index.html` (drag it into the repo's upload page).
4. Go to the repo's **Settings → Pages**.
5. Under "Branch", pick `main` and folder `/ (root)`, then Save.
6. After ~1 minute your site is live at:
   `https://YOUR-USERNAME.github.io/shopall/`

---

## Option 3 — Vercel (fast, great free tier)

1. Create a free account at https://vercel.com
2. Click **Add New → Project → deploy a folder / import**, or install the Vercel CLI:
   ```
   npm i -g vercel
   ```
3. From this folder run:
   ```
   vercel
   ```
4. Follow the prompts. You get a live `https://shopall.vercel.app` style URL.

---

## Which should I pick?

| Goal | Best option |
|---|---|
| I just want a link right now, no signup | **Netlify Drop** |
| I want a permanent free URL I can update | **GitHub Pages** |
| I might add features / a custom domain later | **Vercel** or **Netlify** (with account) |

---

## Notes

- The file that gets served is **`index.html`** (hosts look for this name automatically). `aws.html` is your working copy; keep them in sync, or just edit `index.html` directly from now on.
- Everything runs in the visitor's browser — location detection, price popup, and store links all work on the live site exactly like they do locally.
- A custom domain (e.g. `shopall.com`) can be added later in any of these hosts' settings for a few dollars/year from a domain registrar.
