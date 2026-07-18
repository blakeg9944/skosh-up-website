# Skosh Up — Website

Single-page site for Skosh Up, a soda/swirl trailer in McCall, Idaho.

## Files

- `index.html` — the entire site (HTML, CSS, and the hero photo are all in this one file, so it works if you just double-click it or host it anywhere)
- `assets/sunset.webp` — original hero photo, kept here for reference/reuse

## Viewing it locally

Just open `index.html` in any browser.

## Deploying it

Easiest free options, in order of simplicity:

1. **Netlify Drop** — go to https://app.netlify.com/drop and drag the `index.html` file onto the page. You get a live URL in seconds. Can later attach a real domain.
2. **GitHub Pages** — push this repo to GitHub, then in the repo's Settings → Pages, set the source to the `main` branch. Your site will be live at `https://<username>.github.io/<repo-name>/`.
3. **Vercel** — similar to Netlify, connect the GitHub repo and it deploys automatically on every push.

## Updating content

- Menu items live in the `<main class="menu-section">` block in `index.html`, grouped by category.
- Address/hours are in the `<section class="find">` block.
- Instagram link is in the `find-actions` and footer areas — search for `instagram.com`.

## Notes

- Hours are intentionally left blank/flexible since it's a mobile trailer — the site points people to Instagram for current hours instead.
- The hero photo is embedded directly in `index.html` as base64 so the whole site is one portable file. If you swap in a different image later, use `assets/sunset.webp` as the source and re-encode it into the CSS `background-image` in the `.hero` rule.
