# Monday map updates

Private map: https://damonkeyser-ui.github.io/water6iswet/  
Live file: `index.html` only.

## When
Every Monday **09:00 SAST**. Automation name: water6iswet Monday map update.

## Sources (wider search — use all of these)
1. **https://dankmaps.co.za/map** — primary SA store/event candidates  
2. **https://findweed.co.za** (and **/find-weed**) — SA directory of shops, clubs, CBD  
3. **daggaspot** (and similar SA directories)  
4. **Google** — search queries such as:
   - `"dispensary" OR "cannabis club" OR "private club" Cape Town / Johannesburg / Pretoria / Durban / Gqeberha`
   - `"cannabis club" OR "CBD shop" OR "headshop" London / Manchester / Birmingham / Edinburgh / UK`
   - `"new dispensary" OR "opening soon" South Africa 2026`
5. **Instagram** — public pages/handles for SA & UK shops; posts about openings  
6. **Facebook** — public business pages / local “new business” posts for clubs & shops  
7. **Other web** — news (e.g. Cannabiz Africa), toke.co.za-style lists, official shop sites  

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
