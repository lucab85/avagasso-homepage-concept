# Avagasso homepage concept

A homepage concept for [Avagasso Leadership Coaching](https://www.avagasso.com/) (Sarah Gruneisen), built on a "three planes" layout:

1. **Back:** the name, set as wide as the stage allows.
2. **Middle:** Sarah's cut-out portrait, standing in front of the letters and fading into the page.
3. **Front:** bracketed proof numbers, the tagline and one call to action.

The same idea repeats further down: each proof panel (Landing, The Leap, On stage) has a giant word behind a card or photo, with a badge on the corner.

## Preview

Plain HTML and CSS, no build step and no JavaScript. Serve it over HTTP, because the font and the dragon masks do not load from `file://`:

```sh
python3 -m http.server 8000
# open http://localhost:8000/
```

## What to check before using it

- Every link points to the existing pages on avagasso.com and theleadershiplanding.com. Nothing here replaces the booking, shop or blog.
- Facts are a snapshot of those sites on 15 November 2026 and need Sarah's confirmation: cohort start date (12 January 2027), schedule and price (€987), Leadership Boost and Team Accelerator prices, discovery call (30 min, €5), "5.0 from 40 Google reviews", "188 Draikes", the years in the hero numbers.
- Testimonials and the conference quote are taken from her sites, shortened.
- The portrait is a cut-out of the photo on her site; photos, logo and dragons are hers.
- `<meta name="robots" content="noindex">` is set, so the concept is not indexed if it is ever hosted. Remove it for a real launch.

## Files

- `index.html`: the page.
- `styles.css`: all styles. Colours are the Avagasso palette (ink, green, lime, pink) as custom properties at the top.
- `assets/`: portrait, book photo, dragons, logo and the font (Bricolage Grotesque, SIL Open Font License).
