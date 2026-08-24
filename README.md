# Rasta Roba — Portfolio Site

Live at: https://songwa-cpu.github.io/art-portfolio/

## How to swap in real artwork photos

The 11 tiles on the site currently show placeholder gradients. To replace any of them with a real photo, upload a `.jpg` file to the matching folder **with the exact file name below** — no code editing needed.

1. Go to the repo on GitHub: https://github.com/songwa-cpu/art-portfolio
2. Open the `images` folder, then the sub-folder for the project you want (`unity`, `critical-transformation`, or `divine`)
3. Click **Add file → Upload files**
4. Drag in your photo, renamed to match the slot you're filling (see table below)
5. Commit the change — the live site updates automatically within a minute or two

| Folder | File name | Piece title |
|---|---|---|
| `images/unity/` | `1.jpg` | Goddes Lajja Gauri Creation via Uttanapad |
| `images/unity/` | `2.jpg` | Matondo |
| `images/unity/` | `3.jpg` | Nkyenkye Wo Nafe |
| `images/unity/` | `4.jpg` | Tempted Empress |
| `images/unity/` | `5.jpg` | Woven Excess |
| `images/unity/` | `6.jpg` | Radiant Armor |
| `images/unity/` | `7.jpg` | Unity in Bloom |
| `images/critical-transformation/` | `1.jpg` | Rupture |
| `images/critical-transformation/` | `2.jpg` | Becoming |
| `images/divine/` | `1.jpg` | Nalingi Yo |
| `images/divine/` | `2.jpg` | GEEZUSCRAWLS |

Photos should be portrait orientation (3:4) for the best crop. Any tile without a matching photo just keeps showing its gradient placeholder — nothing breaks.

The piece titles above (`Crowned`, `Regalia`, `Rupture`, etc.) are placeholder names I invented to fill each slot — rename them anytime by editing the `titles` arrays in `index.html`'s closing `<script>` block.

## People photos

Same drag-and-drop upload process as above, into these folders:

| Folder | File name | Used for |
|---|---|---|
| `images/team/` | `songwa.jpg` | Songwa's photo on the `about.html` team page |
| `images/artist/` | `rasta-roba.jpg` | Rasta Roba's photo in the "Read the artist's biography" popup on the homepage |
| `images/modeling/` | `1.jpg`, `2.jpg`, ... | Modeling gallery on `modeling.html` (currently 8 photos, shown full-size in a masonry layout — portrait and landscape shots both display uncropped) |

## Modeling measurements

`modeling.html` has a measurements table (height, bust, waist, hips, dress size, shoe size, hair/eye color) currently showing placeholder dashes — send the real numbers anytime and they'll be filled in.

## Blog posts

Each post is its own page (e.g. `cowrie.html`), long-form/Substack-style: big serif headline, byline row, drop-cap first paragraph, generous body type. It's then listed as a card on `blog.html` via an entry in the `posts` array near the bottom of that file (`title`, `date`, `excerpt`, `link` to the post page, optional `cover` image).

Live: **[Cowrie: The Shells That Echo the Past](cowrie.html)** (Jan 8, 2025) — imported from `Cowrie- The Shells That Echo the Past.docx`.

Adding a post isn't a drag-and-drop upload like photos — send the article text (a Word doc, PDF, or pasted text all work) and Claude will build the page and add the card.

## Shop

`shop.html` lists Rasta Roba's original watercolors, one photo each (full image, not cropped — click to enlarge), with size and price. Currently live: Astray, Clown, Eye Choke, Joi, Slick Sailor (5.8 x 8.3 in) and Prototype (8.3 x 11.7 in). Photos and sizes came from the two "Watercolor..." folders in Downloads; prices were randomly assigned per your instruction (GHC 80/100/120 for the smaller size, GHC 150/200 for the larger) — adjust any of them anytime by editing the `products` array near the bottom of `shop.html`.

To add a new piece: drop the photo in `images/shop/` (any filename), then tell Claude the title, size, and price and it'll be added to the `products` array.

Orders go to WhatsApp number +233 59 427 0853 (set as `WHATSAPP_NUMBER` near the bottom of `shop.html`).

## General uploads

`images/uploads/` is a catch-all folder for any photo that doesn't have an obvious home yet — no naming convention required. Drop files in via **Add file → Upload files** at https://github.com/songwa-cpu/art-portfolio/tree/main/images/uploads, then tell Claude what each one is for (an artwork, a service, a blog cover, etc.) and it'll be moved to the right spot and wired into the site.

## Pages

- `index.html` — the main portfolio
- `services.html` — consultation, photography, commissions, hosting, acting, modeling
- `modeling.html` — Rasta Roba's modeling portfolio and measurements
- `shop.html` — original watercolors, order via WhatsApp
- `blog.html` — journal / stories index
- `cowrie.html` — blog post: Cowrie: The Shells That Echo the Past
- `about.html` — team page

All pages share the same top navigation bar (Work · Services · Shop · Blog · About).

## Analytics

Visitor tracking is live via [GoatCounter](https://www.goatcounter.com/) — dashboard at https://dwatamon.goatcounter.com/. The tracking snippet is on all six pages, right before `</head>`. No cookies, no consent banner needed.

## Custom domain

The page's meta tags reference `art.dwatamon.com`. To point that domain here instead of the `github.io` URL, add a `CNAME` DNS record for `art` pointing to `songwa-cpu.github.io`, then set the custom domain in the repo's **Settings → Pages**.
