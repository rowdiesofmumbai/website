# Rowdies of Mumbai — Website (initial draft)

Official website for **Rowdies of Mumbai**, a Mumbai DJ crew.

- Instagram: [@rowdiesofmumbai](https://www.instagram.com/rowdiesofmumbai/)
- YouTube: [@rowdiesofMumbai](https://www.youtube.com/@rowdiesofMumbai)

## Status

This is a **design-exploration draft**. It holds five candidate visual styles, each with a **Profile** page and a **Videos** page. The theme comes from the crew's profile art: masked, hooded DJs in a neon Mumbai lane, coloured teal and cyan against hot orange and amber.

Once the crew picks a style, it will be built out as the production static site.

## The five styles

| # | Style | Profile | Videos | Idea |
|---|-------|---------|--------|------|
| 01 | Mask Mode | `designs/Main.dc.html` | `designs/MaskMode-Videos.dc.html` | Cinematic neon underground with teal and orange frames. Clicking the hero art plays the theme track. |
| 02 | Galli Wall | `designs/Galli-Profile.dc.html` | `designs/Galli-Videos.dc.html` | Mumbai street wall: stencil type, taped and tilted posters. |
| 03 | Deck HUD | `designs/Deck-Profile.dc.html` | `designs/Deck-Videos.dc.html` | The site looks like DJ software, with decks, waveforms and a track library. |
| 04 | Rave Brutal | `designs/Rave-Profile.dc.html` | `designs/Rave-Videos.dc.html` | Giant type on orange, a hard black grid and tickers. |
| 05 | Night Local | `designs/Local-Profile.dc.html` | `designs/Local-Videos.dc.html` | Local train signage with a "next drop" bar, gigs drawn as stations on a route line and a Devanagari name board. |

## Folder layout

```
designs/          design source for all 10 pages (.dc.html) + canvas.json layout
assets/images/    photos cropped from the Instagram profile and posts
assets/audio/     rowdies-theme.mp3, the track that plays on the Mask Mode hero
```

## Notes

- The `.dc.html` files are Design Component sources from the design canvas. They use `{{…}}` template holes and `<sc-for>` / `<sc-if>` tags, so they need that runtime and **won't render correctly when opened directly in a browser**. The production site will be plain HTML, CSS and JS built from the chosen style.
- Anything in `[BRACKETS]` is a placeholder: DJ names, gig dates, venues, the booking email and set titles.
- The photos are low-resolution crops of Instagram screenshots and will be replaced with originals.

## Next steps

1. The crew picks a style, or mixes elements from several.
2. Add real photos, crew names, gigs and the booking email.
3. Build the production static site, with the Videos page pulling from the YouTube channel.
4. Deploy, for example on GitHub Pages.
