# Waggl Pets

A redesigned storefront for Waggl Pets. It's a single static page: `index.html`, plus the photos and film in `assets/`.

## What's on the page

- The running-dogs film from the live store as the hero, with the store's own line: "Good days. Together."
- A short facts strip: sizes XS to 9XL, made for wet weather, the little white tag
- "Shop by type": rain gear, base layers and bandanas as an index, with a photo that changes as you hover
- A Puddle Parade scroll story that walks through the jacket's details
- A line-up of seven dogs in their bandanas, then every bandana on one swatch wall, grouped into tie-strap and classic (a swipeable row on phones)
- All 12 products from the live Shopify store, with their real prices, colours, sizes, stock and size charts
- A size guide that suggests a size for each product from neck, chest and belly, in inches or centimetres; the size charts switch units too
- A bag that hands off to the live store's checkout through a Shopify cart link
- A newsletter form that signs people up on the live store (it opens the store in a new tab to confirm), and footer links to the store's shipping, returns and contact help

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

A few clean-ups were made to the cutouts themselves: the white neck form is gone from inside the tie-strap loops, polka dots that the cutout had made see-through are white again, and the soft edge along the Samoyed's plaid bandana was repaired. Photos whose original frame cut the dog off at one side sit flush against that side of the tile, so there's no straight edge floating in the middle.

Several store photos had the usual tells of generated images, mostly in the paws (extra claws, melted or toe-less feet). Those photos are now framed chest-up, or cut just below the coat, so the whole garment still shows and the paws don't. Leftover background was cleaned from a few outlines (grass, specks, a ghost tail on the malamute, a smear on the corgi's rump), and the garbled small text under the logo on two Puddle Parade coats was removed (one read "petco").

## Hero film

The film is cut from the store's hero video, using the 720p stream Shopify serves (the highest resolution the upload has). It keeps only the snow, woods and field clips, so no other brand's gear is on screen, and the woods clip is trimmed to its sharpest second. The captions under the film (Snow, Woods, Field) follow the clip that's playing.

- `assets/video/hero-3.mp4` (and `.webm`): 1920 px wide for desktop, upscaled with Lanczos and lightly sharpened.
- `assets/video/hero-3-sq.mp4`: a 1080 px square for phones, the same crop the phone layout shows, so it isn't stretched.
- Both are H.264 High with 4:2:0 colour, the format every phone plays.

It plays muted, pauses when scrolled away, has a Pause/Play control, and doesn't autoplay for people who ask for reduced motion. If a phone won't stream the film from the host, the page downloads it whole and plays it from memory. If the phone won't autoplay video at all (Low Power Mode, some in-app browsers), a looping image of the same clips stands in (`hero-loop-3-sq.webp` on phones, `hero-loop-3.webp` wider).
