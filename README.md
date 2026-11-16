# somethingsticks.com

The website for Something Sticks, LLC. Plain HTML and CSS in one flat folder. No build step, no JavaScript, no trackers, nothing shared with any other project.

## What's here

| File | What it is |
| --- | --- |
| `index.html` | Home page |
| `privacy.html` | Privacy policy (the App Store "Privacy Policy URL") |
| `support.html` | Support page (the App Store "Support URL") |
| `404.html` | Shown for any address that doesn't exist |
| `site.css` | The one stylesheet |
| `young-serif.woff2`, `figtree.woff2` | The two typefaces, self-hosted, with their licenses in the `LICENSE-*.txt` files (SIL Open Font License) |
| `favicon.svg` | Browser tab icon |
| `CNAME` | Tells GitHub Pages the site lives at somethingsticks.com |

To look at it on your own computer, double-click `index.html`. (`404.html` only looks right once it's on the real domain.)

## Publishing a change

1. On GitHub, open the repository, click "Add file", then "Upload files".
2. Drag every file from this folder into the browser and click "Commit changes". Same-named files are replaced.

To take the site offline: Settings, Pages, set Branch to "None", Save. To bring it back, set Branch to `main` and `/ (root)`.

## Before an app is released

- [ ] Add the app to the home page: what it does and how to get it.
- [ ] Fill in the "Our apps" section of `privacy.html` with what the app really collects, why, who can see it, and which service providers store it. Update the date at the top.
- [ ] Confirm `support@somethingsticks.com` and `hello@somethingsticks.com` still reach you.

The copyright year is written out in the footer of each page.
