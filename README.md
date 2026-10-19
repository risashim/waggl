# Waggl Pets

A redesigned storefront for Waggl Pets. It's a single static page: `index.html`, plus the photos in `assets/`.

## What's on the page

- All 12 products from the live Shopify store, with their real prices, colours, sizes, stock and size charts
- "For every kind of day": Outdoors, Urban, At Home and Accessories
- A Puddle Parade feature section
- Shop grid with filters and search
- A fit guide that suggests a size for each product from neck and chest measurements
- A bag that hands off to the live store's checkout through a Shopify cart link

## Run it locally

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Brand system

| Role | Value |
| --- | --- |
| Paper | `#F7F4EF` |
| Ink | `#1C2527` |
| Waggl red | `#D42623` |
| Display type | Funnel Display |
| Body type | Funnel Sans |
| Labels and numbers | Spline Sans Mono |

The signature detail is the small white woven side tag from the bandanas. On the page it's the `.tag` element, sticking out from the edge of each product photo.
