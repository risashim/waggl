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
| Page | `#FFFFFF` white |
| Text | `#1F2747` navy |
| Accent | `#D9272E` Waggl red, used sparingly |
| Soft tiles | blush `#F6E1E1`, powder `#DDE8F4`, butter `#F6EDCB`, sage `#E1EBDA` |
| Headlines | Fraunces, soft cut, with red italic accents |
| Body | Zen Maru Gothic |

Products are shown as background-free cutouts (`assets/cutouts/`) on soft colour tiles. Lifestyle photos live in `assets/img/`. The signature detail is the small white woven side tag from the bandanas: the `.tag` element on every product tile, and the large tag in "Look for the little tag".
