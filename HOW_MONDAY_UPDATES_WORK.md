# Monday map updates

Private map: https://damonkeyser-ui.github.io/water6iswet/
Live file: `index.html` only.

## When
Every Monday 09:00 SAST. Automation: water6iswet Monday map update.

## Sources
- https://dankmaps.co.za/map
- daggaspot
- Instagram / web search (Cape Town dispensary, Johannesburg cannabis club, UK cannabis shop, etc.)

## Add a store only if all of these are true
- Physical storefront in **South Africa** or the **United Kingdom**
- Real street address that geocodes to SA/UK lat/lng
- Not online-only, not USA, not a restaurant / bar unless it is clearly a weed shop
- Not a duplicate of an existing `name` + `city` in STORES
- Prefer complete details: address, phone, website, Instagram, hours

## Store fields
Use the existing STORES schema. New shops get the next integer `id` and go into `NEW_STORE_IDS` so they show under New.
Include when public: name, type, province, city, suburb, address, lat, lng, phone, website, instagram, hours, country, tags.

Types: Dispensary, Private Club, CBD Shop, Grow Shop, Headshop.

## Events
Add upcoming events only (day, month, year, title, place, city, country, lat, lng).
Pins and tab items drop the morning after the event date (`liveEvents()`).

## Do not change
Map look, colours, coverage, visited, hide, Near, or other UI.
Do not wipe `index.html`.
Visited / failure marks stay on the owner’s device (localStorage).

## Commit
`Weekly update: N new stores, M new events (YYYY-MM-DD)`
List what was added in `WEEKLY_UPDATE.md`.
