# Pyrénées + Ordesa + Pays Basque 2026

The trip plan for our road trip, 27 June – 6 July 2026.

**Live site:** https://hughabrown.github.io/pyrenees-2026/

It's a single self-contained `index.html` (map, day-by-day, where we stay, logistics). No build step, no dependencies to install. Edit the file, save, done. The live site rebuilds itself within ~1 minute of any change landing on `main`.

## How to edit the plan

Almost everything you'd want to change lives in three lists near the bottom of `index.html`, in the `<script>` block. You don't need to touch the design or the map code.

| Edit this list | To change |
|---|---|
| `BASES` | Where we sleep each stop (town, dates, hotel pick, blurb) |
| `DAYS` | The day-by-day cards (drive, what to do, where to eat, trail link) |
| `SIGHTS` | The pins on the map (name, lat/lon, type, one-line note) |

Each entry is plain text inside quotes. Copy an existing entry, change the words, keep the commas and brackets where they are. Google Maps links generate automatically from the place name, so you usually don't need a URL.

Marker colours in `SIGHTS` use the `type` field: `green` (hikes/nature), `red` (food), `slate` (town/sight). Night stops are numbered automatically.

## Two ways to make a change

**Easiest, in the browser (no setup):**
1. Open `index.html` here on GitHub.
2. Click the pencil (✎, top right of the file).
3. Make your edits, then "Commit changes" to `main`.
4. Wait ~1 min, refresh the live site.

**Local, if you'd rather use an editor:**
```bash
git clone https://github.com/hughabrown/pyrenees-2026.git
cd pyrenees-2026
# open index.html in your browser to preview as you edit
git add index.html
git commit -m "your change"
git push
```

## The restaurants & pins live in Google Maps too

The curated "Spain 2026" Google Maps list (every restaurant and stop, with notes) is the companion to this site and is the easiest place to add a food spot on your phone. Ask Hugh for edit access to that list if you want to add places without touching the code.
