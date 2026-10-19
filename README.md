# Waggl Pets

A redesigned storefront for Waggl Pets. It's a single static page: `index.html`, plus the photos and film in `assets/`.

## What's on the page

- The running-dogs film from the live store as the hero, with the store's own line: "Good days. Together."
- A short facts strip: sizes XS to 9XL, made for wet weather, the little white tag
- "Shop by kind": rain gear, base layers and bandanas as a type index, with a photo that changes as you hover
- A Puddle Parade scroll story that walks through the jacket's details
- A line-up of seven dogs in their bandanas, then every bandana colour on one swatch wall, grouped into tie-strap and classic
- All 12 products from the live Shopify store, with their real prices, colours, sizes, stock and size charts
- A size guide that suggests a size for each product from neck, chest and belly, in inches or centimetres
- A bag that hands off to the live store's checkout through a Shopify cart link

## Run it locally

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Brand system

The page stays quiet so the dogs can be the cute part. It should feel at home for any age, taste or country.

| Role | Value |
| --- | --- |
| Page | `#FFFFFF` white |
| Studio floor | `#EDEDEA` stone, behind every product and dog |
| Text | `#16181D` ink, `#5E6168` graphite for secondary text |
| Hairlines | `#E2E2DE`, `#C8C9C4` for controls |
| Accent | `#D9262E` Waggl red, only for the logo and a few small marks: the active pin, the fit marker, a saved heart, 9XL in the footer |
| Headlines | Newsreader, light weight, with one italic word where the line needs a little warmth |
| Everything else | Hanken Grotesk; short labels and buttons in spaced capitals, longer labels in sentence case |
| Shape | Square surfaces, 2px corners on controls, no pills, no patterns, no badges |

Every product is shown as a cutout on the stone floor. Dogs photographed from the chest up sit flush on the bottom edge. Full-body dogs stand on the floor with a soft shadow under their paws. Tiles lead with the dog wearing the piece, and the flat shows on hover.

## Bandana photos

The bandana photos are the store's own product photos, cut out onto the stone floor. The embroidered logo is exactly as it appears on the real bandanas.

## Hero film

`assets/video/hero.mp4` (with a WebM copy) is cut from the store's hero video: the snow, woods and field clips only, so no other brand's gear shows on screen. It's re-encoded without sound at 1280 px, and the captions under the film (Snow, Woods, Field) follow the clip that's playing. It plays muted, pauses when scrolled away, has a Pause/Play control, and doesn't autoplay for people who ask for reduced motion.
