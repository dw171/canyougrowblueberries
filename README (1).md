# canyougrowblueberries.com

A blunt, idiot-proof guide to growing blueberries at home outside their
native range. Written from real, multi-year, in-ground results — not a
blog, not a promise.

## Structure

- `index.html` — Page 1: "Can I even do this?" The full build guide —
  reality check, checkbox screener, pH target, berm construction with
  diagram, the non-negotiables (sun, water, fertilizer, weeds, birds,
  deer), honest caveats, and FAQs.
- `varieties.html` — Page 2: "Which variety should I plant?" Zones and
  chill hours explained, pollination requirements by type, and a live
  filterable database of ~49 real blueberry varieties (Northern Highbush,
  Rabbiteye, Southern Highbush, Half-High) — filter by type, zone, season,
  berry size, and bush size.

Both pages share one design system (fonts, colors, components) defined
inline in each file's `<style>` block. No build step, no dependencies —
pure static HTML/CSS/JS.

## Deploying

Static site, zero config needed. Push to GitHub, connect the repo to
Vercel, done. Vercel auto-serves `index.html` as the site root.

## Known gaps / next steps

- The "enter your zip" tool on `varieties.html` is a UI mockup only — it
  currently just scrolls to the manual zone dropdown, which is the real,
  working equivalent for now. Wiring up a real zip → USDA zone → chill
  hours lookup is the natural next step (zone data is a solved problem via
  USDA's public dataset; chill hours are more complex and would need a
  real regional climate data source).
- No photos yet — placeholders were removed until real photos are ready to
  swap in.
- Variety database is comprehensive but not exhaustive — more varieties
  can be added to the `varieties` array in `varieties.html` as they come
  up. Each entry needs: zone range, chill hours, season, berry size, bush
  size, pollination requirement, and a short note.
