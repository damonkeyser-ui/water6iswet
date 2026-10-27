# Monday map updates

Private map: https://damonkeyser-ui.github.io/water6iswet/  
Live file: `index.html` only.

## When
Every Monday **09:00 SAST**. Automation: water6iswet Monday map update.

## Sources
Search all of these for **new** physical shops (and events) in **South Africa and the UK**:

**Directories / maps**
- https://dankmaps.co.za/map  
- https://findweed.co.za (and /find-weed)  
- https://cannamap.club  
- https://thcdirectory.co.za  
- https://toke.co.za  
- https://www.zazamap.com (SA/UK only)  
- daggaspot and similar SA lists  

**Search & social**
- Google Maps (place listings with full address)  
- Google web (“dispensary”, “cannabis club”, “CBD shop”, “opening soon” + city)  
- Instagram & Facebook public business pages / openings  

**UK extras**
- cannabias.io/lounges, cbd-maps.com, cannabishealthnews.co.uk/directory  

If a **new directory site** appears that week, use it and add it to this list next run.

## Add a store only if
- Physical storefront in **SA or UK**
- Real street address that geocodes to SA/UK lat/lng  
- Not online-only, USA, or a non-weed restaurant/bar/nightclub  
- Not a duplicate of existing `name` + `city`  
- Prefer phone / website / Instagram / hours when public  

**Types:** Dispensary · Private Club · CBD Shop · Grow Shop · Headshop  

New shops: next integer `id`, `isNew: true`, existing STORES schema.

## Events
Upcoming only. Drop the morning after the date (`liveEvents()`).

## Do not change
Map UI, colours, coverage, visited, hide, Near. Do not wipe `index.html`.  
Visited data stays on the owner’s device unless they export it.

## Commit
`Weekly update: N new stores, M new events (YYYY-MM-DD)`  
Log what was added in `WEEKLY_UPDATE.md`.
