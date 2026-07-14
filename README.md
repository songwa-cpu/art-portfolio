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
| `images/unity/` | `1.jpg` | Crowned |
| `images/unity/` | `2.jpg` | Regalia |
| `images/unity/` | `3.jpg` | Threaded Gold |
| `images/unity/` | `4.jpg` | Sacred Ornament |
| `images/unity/` | `5.jpg` | Woven Excess |
| `images/unity/` | `6.jpg` | Radiant Armor |
| `images/unity/` | `7.jpg` | Unity in Bloom |
| `images/critical-transformation/` | `1.jpg` | Rupture |
| `images/critical-transformation/` | `2.jpg` | Becoming |
| `images/divine/` | `1.jpg` | Inner Sun |
| `images/divine/` | `2.jpg` | Sacred Thread |

Photos should be portrait orientation (3:4) for the best crop. Any tile without a matching photo just keeps showing its gradient placeholder — nothing breaks.

The piece titles above (`Crowned`, `Regalia`, `Rupture`, etc.) are placeholder names I invented to fill each slot — rename them anytime by editing the `titles` arrays in `index.html`'s closing `<script>` block.

## Custom domain

The page's meta tags reference `art.dwatamon.com`. To point that domain here instead of the `github.io` URL, add a `CNAME` DNS record for `art` pointing to `songwa-cpu.github.io`, then set the custom domain in the repo's **Settings → Pages**.
