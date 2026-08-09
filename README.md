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
| `images/modeling/` | `1.jpg` – `6.jpg` | Modeling gallery on `modeling.html` |

## Modeling measurements

`modeling.html` has a measurements table (height, bust, waist, hips, dress size, shoe size, hair/eye color) currently showing placeholder dashes — send the real numbers anytime and they'll be filled in.

## Blog posts

`blog.html` currently shows an empty state ("New stories are on their way"). Adding a post isn't a drag-and-drop upload like photos — send the post text (and optionally a cover photo) and it'll be added as an entry in the `posts` array near the bottom of `blog.html`, which renders automatically as a card.

## Shop

`shop.html` lists original watercolor pieces. Each product needs 3 photos and each "Order on WhatsApp" button needs a working phone number to actually send anywhere.

| Folder | File name | Used for |
|---|---|---|
| `images/shop/` | `1-1.jpg`, `1-2.jpg`, `1-3.jpg` | Product 1 carousel (3 photos, click the image to cycle through them) |
| `images/shop/` | `2-1.jpg`, `2-2.jpg`, `2-3.jpg` | Product 2 carousel |
| `images/shop/` | `3-1.jpg`, `3-2.jpg`, `3-3.jpg` | Product 3 carousel |

**Still needed:** the WhatsApp number to receive orders — find `const WHATSAPP_NUMBER = "REPLACE_WITH_WHATSAPP_NUMBER";` near the bottom of `shop.html` and swap in the real number, digits only with country code (e.g. `15551234567` for +1 555 123 4567). Product titles are placeholders ("Original Watercolor I/II/III") — send real titles anytime.

## General uploads

`images/uploads/` is a catch-all folder for any photo that doesn't have an obvious home yet — no naming convention required. Drop files in via **Add file → Upload files** at https://github.com/songwa-cpu/art-portfolio/tree/main/images/uploads, then tell Claude what each one is for (an artwork, a service, a blog cover, etc.) and it'll be moved to the right spot and wired into the site.

## Pages

- `index.html` — the main portfolio
- `services.html` — consultation, photography, commissions, hosting, acting, modeling
- `modeling.html` — Rasta Roba's modeling portfolio and measurements
- `shop.html` — original watercolors, order via WhatsApp
- `blog.html` — journal / stories
- `about.html` — team page

All pages share the same top navigation bar (Work · Services · Shop · Blog · About).

## Custom domain

The page's meta tags reference `art.dwatamon.com`. To point that domain here instead of the `github.io` URL, add a `CNAME` DNS record for `art` pointing to `songwa-cpu.github.io`, then set the custom domain in the repo's **Settings → Pages**.
