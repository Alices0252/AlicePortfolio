# Alice — Portfolio

Static portfolio site. No build step, no framework. Just open `index.html`,
or deploy the whole folder as a static site.

## What's here

- `index.html` — home page: hero, Divsly, Soopr, campaign work, about, experience, contact
- `styles.css` — all styling
- `script.js` — mobile menu + footer year only
- `images/` — 13 optimised JPGs picked from `Alice_Portfolio.pdf` (29 Oct 2026).
  Tool logos and the blue background from that PDF were left out.

## Add / replace an image

1. Export from Figma / Photoshop at up to 1600px on the longest side, JPG, ~80% quality.
2. Save it into `images/` with the same file name to replace it, or a new name
   and update the matching `<img src="images/...">` in `index.html`.
3. Keep the `alt` text describing what the image shows.

Soopr still needs an image: save it as `images/soopr-1.jpg` and replace the
placeholder block in `index.html` with an `<img>` like the Divsly one.

## Deploy on Cloudflare Pages (Alice to do)

1. In Cloudflare Dashboard → Workers & Pages → Create → Pages → Connect to Git.
2. Choose the `AlicePortfolio` repository, branch `main`.
3. Framework preset: **None**. Build command: *(leave empty)*.
   Build output directory: `/` (the repository root — `index.html` is there).
4. Save and Deploy. Cloudflare will give you a `*.pages.dev` URL.
5. Optional: add a custom domain in Pages → Custom domains.

Every push to `main` redeploys automatically.

## Before sharing publicly

Check that every image shown is OK to publish — especially Divsly/client
work and any piece using another brand's name or logo. Remove or replace
anything that needs permission first, then push/deploy.
