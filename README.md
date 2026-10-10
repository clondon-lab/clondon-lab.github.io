# charlielondon site

A static site: `index.html` plus `img/` and the resume PDF. No build step.

## Editing
- Timeline entries: the `TIMELINE` array near the bottom of `index.html`.
- Travel captions and photos: the `PLACES` array right below it.
- Swap a photo: drop the new file in `img/` with the same name.

## Preview locally
    python3 -m http.server 8765
Then open http://localhost:8765

## Deploy (Vercel, free)
1. Create a GitHub repo and push this folder to it.
2. On vercel.com: Add New > Project > import the repo. Framework preset: "Other". No build command, output directory `.`
3. Every push to `main` redeploys automatically.

## Custom domain
1. Buy the domain (Vercel, Namecheap, Cloudflare, etc.).
2. Vercel project > Settings > Domains > add it, then set the DNS records Vercel shows.
3. Add the `og:image` meta tag in `index.html` (see the comment there) so the link shows your headshot when pasted.

## Photo credits
- Bahamas: "Beach in front of Royal Towers Atlantis" by Fred Hsu, CC BY-SA 3.0, via Wikimedia Commons (credited on the map card).
- Kennametal logo via Wikimedia Commons; Clarifresh logo and Collars & Co. product photo from the companies' sites.
- Student Body President photo from Boys' Latin's Morehead-Cain announcement.
