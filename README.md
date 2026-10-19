# Waggl Pets

A redesigned storefront for Waggl Pets. It's a single static page: `index.html`, plus the photos and film in `assets/`.

## What's on the page

- The running-dogs film from the live store as the hero, with the store's own line: "Good days. Together."
- "Meet the crew": seven dogs in their bandanas standing in a row. Tap one to shop that bandana
- Three promises, each with an embroidered patch: sized properly, ready for weather, look for the tag
- "What do they need?": rain gear, bandanas, base layers and ponchos
- A Puddle Parade scroll story that walks through the jacket's details
- All 12 products from the live Shopify store, with their real prices, colours, sizes, stock and size charts
- "Pick a bandana": all 24 bandana colourways on one wall
- A fit guide that suggests a size for each product from neck, chest and belly measurements
- A bag that hands off to the live store's checkout through a Shopify cart link

## Run it locally

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Brand system

The look is a classic dog outfitter: navy, sky blue and Waggl red, so it works for every dog, not just the pink-bandana crowd. Pink only appears where a product is actually pink.

| Role | Value |
| --- | --- |
| Page | `#FFFFFF` white |
| Text | `#1B2440` navy |
| Signature blue | `#D6E6F4` sky, with small white dots |
| Product tiles | `#F2F5F8` cloud, the same for every product |
| Bandana wall | `#F3E7C2` butter |
| Base layers | `#DCE6D3` sage |
| Accent | `#D9262E` Waggl red, for italic words, hearts and the polka-dot strips |
| Pattern | Red and white polka dots, from the bandanas, on the top banner and the footer edge |
| Headlines | Fraunces, light weight, soft cut, red italic accents |
| Body | Zen Maru Gothic; buttons and labels in spaced capitals |

Products sit as background-free cutouts (`assets/cutouts/`) on matching tiles. Every dog photo in `assets/studio/` is the dog cut out of its original photo and placed on a plain sky, butter, sage or cloud backdrop with a soft floor shadow and light film grain, so the whole site looks like one photo shoot. The round badges are drawn in SVG to look like embroidered patches. The white woven side tag from the bandanas peeks out of every tile and wags on hover.

## Bandana photos

The bandana photos show the embroidered logo at half its real size. The big logo was removed by copying the fabric from one pattern repeat away, then the same logo was put back smaller. The real bandanas currently ship with the larger logo, so update these photos (or the product) before using them in ads.

## Hero film

`assets/video/hero.mp4` (with a WebM copy) is the store's hero video, re-encoded without sound at 1280 px. It plays muted, pauses when scrolled away, has a pause button, and doesn't autoplay for people who ask for reduced motion.
