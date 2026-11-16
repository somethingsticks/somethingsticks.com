# somethingsticks.com

The website for Something Sticks, LLC. Plain HTML and CSS, all in one flat folder. No build step, no JavaScript, no trackers, nothing shared with any other project.

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
| `.nojekyll` | Tells GitHub Pages to serve the files exactly as they are |

To look at it on your own computer, double-click `index.html`. (`404.html` only looks right once it's on the real domain.)

## Before it goes live

- [ ] `hello@somethingsticks.com` and `support@somethingsticks.com` exist and reach you. Both are printed on the site.
- [ ] Read `privacy.html` against what the app really does. The "Our apps", "What we don't do", "Who helps us run things" and "Keeping and deleting data" sections are a first draft written from the three features (time clock, messaging, shared files). If the app collects anything else, sends text messages, uses analytics or crash reporting, or signs people in some other way than email, change the page to match before submitting to the App Store.
- [ ] If the site ends up hosted somewhere other than GitHub Pages, change the second paragraph under "This website" and the "Who helps us run things" line in `privacy.html`, and delete `CNAME` and `.nojekyll`.

## Putting it on GitHub Pages

1. Create a GitHub organization for the company (for example `something-sticks`) and a public repository in it (for example `somethingsticks.com`).
2. Put these files in the repository's `main` branch, at the top level.
3. In the repository: Settings, then Pages. Under "Build and deployment" choose "Deploy from a branch", branch `main`, folder `/ (root)`.
4. On the same screen, set the custom domain to `somethingsticks.com`.
5. At Porkbun, open DNS for somethingsticks.com and add:

   | Type | Host | Answer |
   | --- | --- | --- |
   | A | (blank) | 185.199.108.153 |
   | A | (blank) | 185.199.109.153 |
   | A | (blank) | 185.199.110.153 |
   | A | (blank) | 185.199.111.153 |
   | CNAME | www | `<organization-name>.github.io` |

   Delete Porkbun's default parking records for the bare domain and `www` first. Leave the MX and TXT records for email alone. Add these by hand rather than with Porkbun's one-click "GitHub" button, which rewrites the domain's DNS records.
6. Back on the Pages screen, wait for the DNS check to pass, then tick "Enforce HTTPS".

## Changing things

Edit the HTML, commit, push. The site updates a minute or so later.

The copyright year is written out in the footer of each page.
