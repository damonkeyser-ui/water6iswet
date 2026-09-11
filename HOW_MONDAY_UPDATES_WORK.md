# How Monday updates work

This is the test so you can see the process on GitHub.

## 1. Search
Every Monday I check:
- https://dankmaps.co.za/map
- https://daggaspot.co.za
- Instagram + public websites

Only **physical shops in South Africa or the UK** with a real address get added.

## 2. Verify
A shop is added only if it has:
- Name
- Street address + city
- Map pin (lat/lng)
- Instagram and/or website when public
- Phone when public

Skipped: online-only, USA, duplicates already on the map.

## 3. Update the map file
New shops go into `index.html` and into the **New** tab.
New events go on the Events tab + pink pins.
Events disappear after their date.

## 4. Push to this repo
A commit appears here on **main**.
If GitHub Pages is on, the live site updates after a minute.

## This test (11 Sep 2026)
Sources checked: DankMaps, DaggaSpot Johannesburg/Cape Town/Sandton, Instagram.
Most listed spots (Bud Box Honeycrest, Herb Haus, Dazed and Blazed, Canna Studio, Seknd Nature, etc.) were **already on the map**.

**Added this run:** Highgrounds BLVD (see `STORES_ADDED.json`).

## What you do
1. Open https://github.com/damonkeyser-ui/water6iswet
2. Refresh — you should see this file + `STORES_ADDED.json` + `WEEKLY_UPDATE.md`
3. To put the full map live, upload the latest `water6iswet.html` as `index.html` (large file).
4. Message **Monday update** each week.
