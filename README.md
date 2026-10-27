# Everlume Health website mock-up

Static design mock-up for Everlume Health, a women's health clinic in Farmington, Utah. It's built to be served from GitHub Pages at `/everlume-health/` (Settings → Pages → Deploy from branch → `main` / root).

## Pages

| Template | URL |
| --- | --- |
| Home | `/everlume-health/` |
| Condition | `/everlume-health/conditions/perimenopause/` |
| Sub page (grandchild) | `/everlume-health/symptoms/hormones-energy/hot-flashes/` |
| Location | `/everlume-health/locations/farmington-ut/` |
| Site blueprint | `/everlume-health/blueprint/` |

Any other menu link opens `planned/`, which shows the clean URL the page will use (`404.html` redirects there).

## Navigation

Symptoms, Solutions, Learn and About are cascading menus, three levels deep: parent, then child, then grandchild in a side flyout, the way a WordPress menu nests. Example: Symptoms › Hormones and Energy › Hot Flashes. Life Stages and Conditions stay as grouped mega menus. On mobile the same structure becomes a nested accordion. `assets/site.js` highlights the current page and its parent items in the menu.

## Assets

- Logo and favicon are in `assets/brand/`, cut from the client's logo file.
- Photos load from their Unsplash originals (sized and cropped by URL, served as WebP/AVIF).

All pages are `noindex, nofollow` while this is a staging mock-up.
