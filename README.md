# Local SERP Viewer

**See Google the way your customer sees it.**

Type in a town and a search, and this free tool opens Google's results set to
that town — using Google's own location parameter — so you can look at the
results page the way someone standing in that town would see it.

Try the live version: https://leadlabhq.com/tools/local-serp-viewer/

## What it is (and what it isn't)

- It is a **viewer**. It sets the search location to the town you pick and
  opens the real Google results page.
- It is **not a rank tracker**. Google still weighs the exact spot, the time,
  and — if you are signed in — your history. Two looks an hour apart can
  differ. Use it to see what a customer in that town is looking at, not as a
  position report.

## How it works

One self-contained page (`index.html`). No build step, no server, no accounts,
no tracking. Open the file in a browser and it works.

1. You type a town and a search.
2. The page looks the town up with OpenStreetMap's Nominatim service to get
   its map coordinates.
3. It builds a Google search link carrying Google's own location parameter
   (the `uule` parameter) for that spot, and opens it.

## Data note

Place lookup uses OpenStreetMap data via the Nominatim API. OpenStreetMap
data is © OpenStreetMap contributors and is available under the Open Database
License (ODbL): https://www.openstreetmap.org/copyright

## License

MIT — see `LICENSE`. Built by [The Lead Lab](https://leadlabhq.com).
