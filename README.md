# Geo-Intelligence Report — Southeastern Nantucket

An interactive satellite map dossier of a surficial-geology field survey along the
Sconset / Sankaty Head shore. Each photo is pinned at the exact GPS coordinates
read from the image, with its own title, description, and optional video link.

## Files
```
index.html      ← the whole app (open it / edit it here)
images/         ← all the photos (add yours here)
```

## Edit titles & descriptions
Open `index.html` and scroll to the **SPECIMEN REGISTER** list near the top.
Each photo is one block. Fill in `title`, `description`, and (optionally) `video`:

```js
{ file:"IMG_0541.jpeg", type:"specimen",
  title:"Garnet sand at low tide",
  description:"First line.\nSecond line.",
  video:"https://youtu.be/XXXXXXXX",
  lat:41.261008, lon:-69.962661, alt:3.9, time:"2026-06-19 16:20" },
```

## Add more photos
1. Drop the image into the `images/` folder.
2. Copy a block in the SPECIMEN REGISTER, change `file:` to the new filename, write your text.
3. If the photo still has its phone GPS data, you can **delete** the `lat/lon/alt/time`
   lines — the page extracts them from the photo automatically. No GPS? Just type
   `lat:` and `lon:` yourself.

`type:"specimen"` = numbered red pin · `type:"reference"` = dark pin (maps, diagrams).

## Publish a shareable link (GitHub Pages — free)
1. Create a repo at [github.com](https://github.com) → **New repository** (Public).
2. **Add file → Upload files** → drag in `index.html` **and** the `images` folder. Commit.
3. **Settings → Pages** → Source: *Deploy from a branch*, Branch: **main** / **root**. Save.
4. After ~1 min your live link is `https://<your-username>.github.io/<repo>/` — share it.

To update later, edit `index.html` in the repo (pencil ✎ → Commit) or re-upload. The
link refreshes automatically.

---
Imagery © Esri (World Imagery / Topographic). Map by Leaflet.
