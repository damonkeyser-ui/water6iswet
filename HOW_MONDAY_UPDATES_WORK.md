# Monday map updates

Private map: https://damonkeyser-ui.github.io/water6iswet/  
Live file: `index.html` only.

## When
Every Monday **09:00 SAST**. Automation name: water6iswet Monday map update.

## Sources (wider search — use all of these)
1. **https://dankmaps.co.za/map** — primary SA store/event candidates  
2. **https://findweed.co.za** (and **/find-weed**) — SA directory of shops, clubs, CBD  
3. **https://cannamap.club** — large SA clubs/dispensaries map (CannaMapZA)  
4. **https://thcdirectory.co.za** — clubs, dispensaries, grow shops, events  
5. **https://toke.co.za** — social clubs / head shops / business listings  
6. **https://www.zazamap.com** — clubs map (SA + other countries; only SA/UK)  
7. **daggaspot** (and similar SA directories)  
8. **Google Maps** — public place listings for cannabis club / dispensary / CBD shop / headshop in SA & UK cities (name + full address + phone). Prefer a second source.  
9. **Google** (web) — city queries and “new dispensary” / “opening soon”  
10. **Instagram** — public pages/handles; openings  
11. **Facebook** — public business pages / local new-business posts  
12. **UK directories** when relevant: cannabias.io/lounges, cbd-maps.com, cannabishealthnews.co.uk/directory  
13. **Other web** — news (e.g. Cannabiz Africa), official shop sites  

Also note any **new directory sites** found that week and fold them into this list next run.

Always cover **both South Africa and the United Kingdom**.

## Add a store only if ALL of these are true
- Physical storefront in **South Africa** or the **United Kingdom**
- Real street address that geocodes to SA/UK lat/lng
- Not online-only, not USA, not a restaurant/bar/nightclub unless it is clearly a weed/CBD/grow/head shop or private cannabis club
- Not a duplicate of an existing `name` + `city` in STORES
- Prefer complete details: address, phone, website, Instagram, hours

## Store fields
Use the existing STORES schema. New shops get the next integer `id` and `isNew: true` (so they show under New).  
Include when public: name, type, province, city, suburb, address, lat, lng, phone, website, instagram, hours, country.

**Types:** Dispensary, Private Club, CBD Shop, Grow Shop, Headshop.

## Events
Add upcoming events only (day, month, year, title, place, city, country, lat, lng).  
Pins and tab items drop the morning after the event date (`liveEvents()`).

## Do not change
Map look, colours, coverage, visited, hide, Near, or other UI.  
Do not wipe `index.html`.  
Visited / failure marks stay on the owner’s device (localStorage).  
Do not put personal visit data into the shared repo unless the owner exports it on purpose.

## Commit
`Weekly update: N new stores, M new events (YYYY-MM-DD)`  
List what was added in `WEEKLY_UPDATE.md` (run log only — not the same as this instruction file).
