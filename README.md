# Rasta Roba — Portfolio Site

Live at: https://songwa-cpu.github.io/art-portfolio/

## How to swap in real artwork photos

The 12 tiles on the site currently show placeholder gradients. To replace any of them with a real photo, upload a `.jpg` file to the matching folder **with the exact file name below** — no code editing needed.

1. Go to the repo on GitHub: https://github.com/songwa-cpu/art-portfolio
2. Open the `images` folder, then the sub-folder for the vessel you want (`remembrance`, `transformation`, or `divine`)
3. Click **Add file → Upload files**
4. Drag in your photo, renamed to match the slot you're filling (see table below)
5. Commit the change — the live site updates automatically within a minute or two

| Folder | File name | Piece title |
|---|---|---|
| `images/remembrance/` | `1.jpg` | Ancestral Echo |
| `images/remembrance/` | `2.jpg` | The Remembering |
| `images/remembrance/` | `3.jpg` | Mother Tongue |
| `images/remembrance/` | `4.jpg` | Roots of Light |
| `images/transformation/` | `1.jpg` | Vessel I |
| `images/transformation/` | `2.jpg` | Threshold |
| `images/transformation/` | `3.jpg` | Communion |
| `images/transformation/` | `4.jpg` | Return |
| `images/divine/` | `1.jpg` | Inner Sun |
| `images/divine/` | `2.jpg` | Divine Current |
| `images/divine/` | `3.jpg` | The Unseen |
| `images/divine/` | `4.jpg` | Sacred Thread |

Photos should be portrait orientation (3:4) for the best crop. Any tile without a matching photo just keeps showing its gradient placeholder — nothing breaks.

## Custom domain

The page's meta tags reference `art.dwatamon.com`. To point that domain here instead of the `github.io` URL, add a `CNAME` DNS record for `art` pointing to `songwa-cpu.github.io`, then set the custom domain in the repo's **Settings → Pages**.
