# Jaswant & Divya Darshini · 3D Wedding Invitation

A static site: `index.html` plus a link-preview image. There is no build step.

## Files
- `index.html`: the invitation, a 3D temple scene built with Three.js and Tailwind (both loaded from a CDN)
- `og-image.jpg`: the 1200×630 preview card shown when the link is shared on WhatsApp or social media
- `vercel.json`: Vercel settings

## Edit details
Open `index.html` and find `window.CONFIG`. Update the muhurtham time (`dateISO`, `muhurthamText`) and the hosts' names (`hosts`).

## Deploy to Vercel
**Option A: CLI**
```bash
npx vercel          # first run: log in and accept the defaults
npx vercel --prod
```

**Option B: GitHub**
Push this folder to a GitHub repo. Then go to vercel.com → Add New → Project → Import the repo → Framework preset "Other" → Deploy.

## After the first deploy
1. In `index.html`, replace both `SITE_URL` placeholders with the live URL (for example `https://jaswant-divyadarshini.vercel.app`) and redeploy. Without this, the WhatsApp preview image won't show.
2. Optional: in Vercel → Project → Settings → Domains, rename the free subdomain or connect a custom domain.
3. Paste the link into WhatsApp once to check that the preview card appears before sending it to guests.
