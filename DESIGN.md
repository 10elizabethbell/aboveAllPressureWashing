---
name: Above All Pressure Washing & Shrink Wrapping
description: Phone-first pitch one-pager where the visitor's finger is the pressure-washer jet.
colors:
  navy: "#26215e"
  navy-2: "#2f2a72"
  ink: "#1e1a4d"
  ink-soft: "#4a4775"
  sky: "#4aa3dc"
  sky-2: "#8fcdf0"
  sky-ink: "#2a7fbf"
  mist: "#eef5fb"
  mist-2: "#dfeaf4"
  on-navy-soft: "#c9c8ea"
  white: "#ffffff"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.55rem, 11.2vw, 5.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2rem, 8.6vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(1.35rem, 6vw, 1.9rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 800
    lineHeight: 1.2
rounded:
  focus: "6px"
  card: "18px"
  film: "24px"
  pill: "999px"
spacing:
  gutter-phone: "16px"
  gutter-desk: "32px"
  section-phone: "44px 0 52px"
  section-desk: "64px 0 76px"
  column-gap: "56px"
  container: "1180px"
components:
  button-primary:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.white}"
    rounded: "{rounded.pill}"
    padding: "0 22px"
    height: "58px"
  button-primary-hover:
    backgroundColor: "{colors.navy-2}"
  button-secondary:
    backgroundColor: "{colors.white}"
    textColor: "{colors.navy}"
    rounded: "{rounded.pill}"
    padding: "0 22px"
    height: "58px"
  button-secondary-hover:
    backgroundColor: "{colors.mist}"
  button-primary-on-navy:
    backgroundColor: "{colors.white}"
    textColor: "{colors.navy}"
    rounded: "{rounded.pill}"
  button-primary-on-navy-hover:
    backgroundColor: "{colors.mist}"
  top-call:
    backgroundColor: "{colors.mist}"
    textColor: "{colors.navy}"
    rounded: "{rounded.pill}"
    padding: "0 14px"
    height: "44px"
  chip-service-tag:
    textColor: "{colors.sky-2}"
    rounded: "{rounded.pill}"
    padding: "4px 10px"
  photo-tag-after:
    backgroundColor: "{colors.white}"
    textColor: "{colors.navy}"
    rounded: "{rounded.pill}"
    padding: "5px 11px"
  card-quote:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "20px 20px 18px"
  step-dot:
    backgroundColor: "{colors.white}"
    textColor: "{colors.navy}"
    size: "48px"
---

# Design System: Above All Pressure Washing & Shrink Wrapping

## Overview

**Creative North Star: "The Wall Mid-Wash"**

The page is vinyl lap siding under a mildew film, and the visitor's finger is the pressure-washer jet that cuts it clean. Everything else is built from that same job site: water sheeting down between sections, a white jet with spray droplets, a wet sheen that dries, and glossy shrink film for the off-season. The palette is lifted straight from the owner's logo (indigo-navy wordmark, sky-blue water swoosh), so the page reads as his business before it reads as a design.

Density is phone-first and loud: heavy uppercase display type in promo-flyer voice, sentence-case body, big pill buttons for thumbs, and light mist grounds alternating with indigo-navy bands. Motion is material, not decorative: every moving thing is water or film, all driven by one shared animation loop that pauses off screen and holds a still frame under reduced motion.

**Key Characteristics:**
- Logo-derived indigo-navy and sky blue; navy stands in for black everywhere.
- Mist / navy band alternation, joined by animated three-line water-sheet seams.
- System font stack at weight 900, uppercase, tight leading for all headings (owner's house style).
- Pills for every interactive or tag element; 18px rounded cards for content.
- Soft, navy-tinted shadows with negative spread; nothing hard-edged.
- Two interactive materials: the wash canvas (hero + close) and the shrink-film sheen.

## Colors

A two-hue logo palette: indigo-navy for weight and text, sky blue for water, cool mist for clean siding. All tokens live on `:root` at the top of the `<style>` block.

### Primary
- **Wordmark Indigo** (navy): the dark ground of the services, area and footer bands, primary button fill, and heading color on light grounds. The page's black.
- **Pressed Indigo** (navy-2): primary button hover only.

### Secondary
- **Swoosh Sky** (sky): water. The middle seam line, the hose line in "How a job goes", focus rings, service-row arrow hover, the promise periods, reviews scrollbar. Decorative or large only; on light grounds it fails text contrast.
- **Spray Sky** (sky-2): light water on navy. Service tags, the "&" in the area headline, text selection, the slider jet's highlight.
- **Sky Ink** (sky-ink): the sky hue darkened to pass 3:1 on mist. Use it whenever sky has to be read on a light ground (hero "new", hero meta icons).

### Neutral
- **Ink** (ink): body text on light grounds and inside the shrink-film panel.
- **Soft Ink** (ink-soft): ledes, pitch, meta, step copy, review source lines.
- **Clean Siding Mist** (mist): page background and light bands; hover fill for white buttons.
- **Deep Mist** (mist-2): placeholder fill behind photos while they load.
- **Soft Lilac** (on-navy-soft): secondary text on navy (ledes, service descriptions, footer).
- **White** (white): cards, top bar, photo frames, buttons on navy. Written as literal `#fff` in the CSS; the `--white` token exists but isn't referenced.

### Named Rules
**The Never-Black Rule.** Dark means Wordmark Indigo. No `#000` grounds or text. Black-alpha shadows are only allowed on top of navy, where a navy tint wouldn't show.

**The Sky-Ink Rule.** Sky blue on a light ground is decoration. If it carries words or a meaningful icon, switch to sky-ink.

**The Logo-Red Rule.** The wand red belongs to the logo image. `--red` is declared but unused. Leave it that way unless it gets a real, single-purpose role.

## Typography

**Display Font:** system UI stack (`--font`)
**Body Font:** the same stack

**Character:** One family. Weight and case do all the work: 900 uppercase headings with tight leading and slight negative tracking read like the owner's promo flyers, set against relaxed 17px sentence-case body. The system stack is the owner's explicit house style, not a fallback. Don't swap in a webfont.

### Hierarchy
- **Display** (900, clamp 2.55 to 5.6rem, 0.95): the hero headline only. The emphasised word goes in sky-ink.
- **Headline** (900, clamp 2 to 3.6rem, 0.95): section h2s. Two louder siblings sit on navy: the area headline (clamp 2.2 to 4.4rem) and the promise list (clamp 1.8 to 3rem, line-height 1.05, each line ending in a sky period).
- **Title** (900, about 1.25 to 2.6rem depending on container): h3s. Service rows (1.35 to 1.9rem), steps (1.25 to 1.6rem), reviews heading (1.5 to 2.2rem), shrink-film heading (1.7 to 2.6rem).
- **Body** (400, 17px, 1.55): copy. Ledes cap at 60ch, service and step copy at 52ch, the hero pitch at 34ch on phones (scales 16 to 20px).
- **Label** (700 to 800, 12 to 15px): buttons (800, 17px), meta row, chips, counters. Uppercase only on the before/after photo tags (12px, 0.05em).

### Named Rules
**The Shout-and-Explain Rule.** All h1 to h3 are 900 uppercase at 0.95 leading. Everything else stays sentence case. The base heading rule is in the global `h1,h2,h3` declaration; per-heading sizes sit on each component's selector.

**The Balanced-Headline Rule.** Headings use `text-wrap: balance`. Write headlines short enough that the balancing does the layout.

## Layout

One centred container (max 1180px, 16px gutters, 32px from 760px) inside full-bleed colour bands. Sections pad 44/52px on phones and 64/76px from 760px. Band order is mist, navy, mist, mist, navy, mist, then navy footer. Every mist/navy change goes through a seam.

Breakpoints (in the `<style>` media queries): **760px** gives wider gutters, side-by-side hero buttons, taller seams (64px) and a two-up review row. **1000px** is desktop: hero splits copy | wash panel (1.05fr / 1fr, max 1440px, wash panel at least 560px tall), and the services, proof, how and area sections become two-column grids with a 56px gap (36px for proof). Phone-only and desktop-only text switch on the `.mob` / `.desk` classes; desktop buttons show the phone number.

The phone sticky bar (Call | Text) sits fixed at the bottom. It only appears while neither the hero buttons nor the closing buttons are on screen, and it writes `--bar-h` so the footer clears it.

**The Thumb-Reach Rule.** Every tap target is at least 44px tall. Primary actions are 58px pills (54px in the sticky bar), stacked full-width on phones.

## Elevation & Depth

Depth is soft and ambient. Every shadow has a large blur, a negative spread and a navy tint (`rgba(38,33,94,…)`), so things sit just above the mist rather than casting hard edges. Photo frames add depth with a 6px white border plus the shared `--shadow`. Full values are in the sidecar.

### Shadow Vocabulary
- **Frame lift** (`--shadow`: `0 10px 30px -12px rgba(38,33,94,.35)`): before/after photo frames.
- **Button lift** (`0 8px 20px -8px rgba(38,33,94,.6)`): primary button on light grounds. On navy: `0 8px 22px -8px rgba(0,0,0,.45)`.
- **Card rest** (`0 8px 24px -16px rgba(38,33,94,.45)`): review cards.
- **Film float** (`0 18px 40px -18px rgba(0,0,0,.5)`): shrink-film panel on navy.
- **Handle** (`0 6px 14–16px -4/-6px rgba(20–38,…,.5)`): slider knob, step dots, wash hint.
- **Bar** (`0 -8px 24px -12px rgba(38,33,94,.45)`): phone sticky bar, casting upward.

**The Indigo Shadow Rule.** Shadows on light grounds are navy-tinted with negative spread. Hover lifts by `translateY(-2px)`, not by a bigger shadow.

## Shapes

Three corner levels: **pills** (999px) for everything you tap or read as a tag (buttons, call chip, service tags, film items, photo tags, wash hint and score, sticky-bar buttons); **18px** (`--radius`) for content containers (photo frames, slider, review cards); **24px** for the shrink-film panel only. Circles for the service arrow (44px), step dots and slider knob (48px). Focus rings are a 3px sky outline at 3px offset with a 6px radius.

Lines are water: the seams are three wavy strokes (pale sky, sky, white), and the steps hang off a 6px rounded sky "hose" line. Service rows are separated by 1px white-18% hairlines on navy.

## Components

### Buttons
Big confident pills that always come in a pair: Call (primary) and Text (secondary), same height, same 2px outline.
- **Shape:** pill, min-height 58px, 0 22px padding, 800 weight 17px label with a 22px stroke icon.
- **Primary / Secondary on mist:** navy fill with white text / white fill with navy text, both with a navy 2px border.
- **On navy** (`.on-navy` parent): primary turns white with navy text, secondary turns transparent with a white border.
- **States:** hover (hover devices only) lifts 2px and shifts fill; active scales to 0.97; motion is `.2s cubic-bezier(.2,.8,.2,1)`.

### Chips
- **Service tags** (on navy): 13px 700, sky-2 text on 14% sky-2 tint.
- **Film items** (in the shrink-film panel): 14px 800 navy on 70% white.
- **Photo tags:** "Before · …" in 82% ink with white text, "After" in white with navy text. 12px uppercase, pinned top-left / top-right.

### Cards / Containers
- **Review cards:** white, 18px corners, card-rest shadow, 20px padding. They sit in a horizontal snap-scroll row (86% / 44% / 31.5% wide by breakpoint) with the name in navy 800 pinned to the bottom.
- **Photo frames:** 18px corners, 6px white border, frame-lift shadow, deep-mist fill while loading.

### Navigation
No nav menu. The top bar is white, 68px (84px on desktop), with the logo on the left and a mist "Call" pill on the right. On phones the sticky Call | Text bar takes the place of navigation.

### Service rows
Full-width text links on navy. A 900 uppercase title, soft-lilac description and tags, and a 44px circular arrow that fills sky and slides 4px right on hover or press. Each row opens a pre-filled text naming the service (`data-sms`).

### Wash panel (signature)
A canvas of lap siding under procedural mildew. Pointer or touch cuts it clean with a fan-shaped jet, impact mist, droplets and a drying wet sheen. When idle, the wand sweeps on its own, and grime grows back in patches. A "% clean" pill appears after first touch and the hint pill fades. There are two instances: the **hero** (8px white "trim" edge on top on phones, on the left on desktop) and the **close** strip (starts 58% clean, never regrows, so the page ends on the payoff). The CSS fallback before JS is a striped-siding gradient under a green film.
- **Tunables:** the `CFG` object at the top of the main `<script>`: `JET_RADIUS` (30), `REGROW` (0.0045), `AUTO_SPEED` (1.0), `IDLE_RETURN_MS` (1800), `DROPS_PHONE` / `DROPS_DESK` (90 / 240). Siding and grime colours are hard-coded in the wash panel IIFE's `build()`. Panel heights are in CSS (`.wash`, `.close-wash`).

### Seams (water-sheet dividers)
44px (64px from 760px) SVG dividers drawn by the seams IIFE. Three moving strokes, and the lower colour fills under the middle line. Speed and swell come from `CFG.SEAM_SPEED` (1.0) and `CFG.SEAM_AMP` (0.34). Each seam's top/bottom colours are hex literals in its `data-top` / `data-bottom` attributes. If you change `--navy` or `--mist`, update those and the seam stroke colours in the IIFE too.

### Shrink-film panel
A 24px rounded panel of pale-blue film gradients with a white radial sheen at `--mx` / `--my`. The sheen follows the pointer and drifts on its own when idle. Navy heading, ink copy, white film-item chips and a primary Text button. It's the only light surface inside the navy services band.

### Before/after slider
A 4:3 framed slider. The after image clips at `--pos`, the divider is a 4px white-to-sky water jet, and the knob is a 48px white circle. It responds to pointer drag, horizontal-only touch drag and arrow keys (5% steps). The siding pair sits side by side instead because the photos are from different angles.

## Do's and Don'ts

### Do:
- **Do** take every colour from the `:root` tokens. Use navy for anything dark and sky-ink for sky that carries meaning on mist.
- **Do** alternate mist and navy bands and join every change with a seam.
- **Do** set every heading in 900 uppercase at 0.95 leading, and keep body copy sentence case at 17px / 1.55.
- **Do** use pills for interactive elements and tags, 18px corners for content cards.
- **Do** keep Call and Text as a matched pair (same height and border) everywhere they appear.
- **Do** run any new motion through the shared `Loop`, pause it off screen, give it a reduced-motion still frame, and use only transform, opacity or canvas.
- **Do** make new moving elements out of the world's materials: water, jet, droplets, siding, film.

### Don't:
- **Don't** introduce black grounds or black text (The Never-Black Rule).
- **Don't** load a webfont. The system stack is the owner's house style.
- **Don't** use the logo red as a UI colour.
- **Don't** put small uppercase tracked labels (eyebrows) above headings. The shrink-film eyebrow was removed in review, and the leftover `.ba-label` rule is dead CSS.
- **Don't** use hard-offset or black shadows on light grounds.
- **Don't** add a second animation loop or per-element `requestAnimationFrame`.

## Where to edit

| Want to change | Where |
|---|---|
| Brand colours, card radius, frame shadow, font stack | `:root` at the top of `<style>` |
| Heading weight, case, leading | the global `h1,h2,h3` rule |
| Individual heading sizes | each component's selector (`.hero h1`, `.sec h2`, `.svc h3`, …) |
| Section padding, gutters, breakpoints | `.sec`, `.wrap`, and the `760px` / `1000px` media queries |
| Button size, colour, hover | the Buttons block in `<style>` |
| Jet size, grime regrowth, idle sweep, droplets, seam speed and swell | `CFG` at the top of the main `<script>` |
| Seam colours | `data-top` / `data-bottom` on each seam `<div>`, plus the stroke colours in the seams IIFE |
| Siding / mildew colours | `build()` in the wash panel IIFE |
| Shrink-film gradient and sheen | `.wrapfilm` in CSS; idle drift in the shrink-film IIFE |
| Phone number, business name | `CFG.PHONE`, `CFG.BUSINESS`, plus the `tel:` / `sms:` hrefs in the markup |


## Update: hero is the wall (2026-10-08)
Header + hero + first seam sit inside `.wall` (siding as a CSS repeating gradient, 22px boards). Two canvases cover it, both `pointer-events:none`: `.grime` (low-res, CSS-scaled, `mix-blend-mode:multiply`, so the grime darkens the text and buttons under it rather than hiding them) and `.fx` (jet, mist and droplets at device resolution). The seam sits above both (z-index 5). Mouse: press and drag to spray; hover only pushes droplets. Touch: the finger sprays. Grime darkness for the wall is the `overlay` lift factors in `build()`; the wall jet is 1.4x `CFG.JET_RADIUS` on desktop.
