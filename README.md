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
| Text | `#1E2645` navy |
| Signature pink | `#F5DADA` blush, with tiny white polka dots |
| Product tiles | `#F8F2F0` shell, the same for every product |
| Rain section | `#DCE6F1` powder blue |
| Accent | `#D7262D` Waggl red, for italic words and hearts only |
| Headlines | Fraunces, light weight, soft cut, red italic accents |
| Body | Zen Maru Gothic; buttons and labels in spaced capitals |

Products sit as background-free cutouts (`assets/cutouts/`) on matching tiles, and the photo of a dog wearing it fades in on hover. "Best dressed" uses pop-out portraits where each dog's head rises above its circle. The signature detail is the white woven side tag from the bandanas, which peeks out of every tile and wags on hover.
