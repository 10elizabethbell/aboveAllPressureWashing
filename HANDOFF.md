# Above All Pressure Washing & Shrink Wrapping — handoff at ~60%

**Live file:** index.html · **Repo:** https://github.com/10elizabethbell/aboveAllPressureWashing · **Built:** 2026-10-08 from Muse brief (run 2026-10-08, FB group "Ocean county small businesses and services.")

## What's built
- **Update 2026-10-08 (Ellie's request):** the whole top of the page (header + hero, down to the first blue waves) is now one dirty siding wall. Grime sits over the logo, headline and buttons (multiply blend, so they stay readable and tappable). The idle wand washes across everything, and click-and-drag (desktop) or a finger (phone) takes over. Hover alone only nudges the spray. The separate hero wash panel is gone. The hero Text button is now "Text Sean" (it was "Text Sean a photo"). Code: `.wall` CSS, and `Panel()` with `overlay` true in the wash script. Boards are wide (`--board`: 40px on phones, 56px at 760px and up) with soft shadow seams, and the mildew under each lip is weaker, so the seams don't cut through the copy.
- **World:** a wall mid-wash. Vinyl lap siding under a mildew film; the visitor's finger (or mouse) is the pressure-washer jet that cuts it clean, with spray droplets and a wet sheen that dries. When idle, the wand sweeps on its own in horizontal passes. Grime creeps back in patches so the panel never stays finished. A "% clean" counter appears once someone touches it.
- **Colors** come from Sean's real logo: indigo-navy `#26215e` (dark grounds, never black), sky blue `#4aa3dc` (water), pale "clean siding" mist `#eef5fb` (light grounds).
- **Sections:** top bar with logo + Call → hero ("Like a whole new home.", their own line) with Call + Text buttons and the wash panel right under them → services on navy (power washing, soft washing, gutter cleaning; each whole row texts Sean with the service named) then a second group, "Boats and equipment." (shrink wrapping: boats & watercraft, hot tubs, outdoor furniture & grills, equipment; each row texts Sean with the item named). The blue shrink-wrap card was removed on Ellie's request → proof, now titled "Sean's work." (draggable siding before/after with a water-jet divider, a 6-photo shrink-wrap gallery, a link to Sean's Facebook for more work, 5 testimonials in a swipe row) → how a job goes (hose line, 3 steps) → Ocean & Monmouth + their promise "detailed. organized. honest. fast." → close (logo, name, Call/Text/email; the bottom wash strip was removed on Ellie's request) → footer with "Demo one-pager — free sample."
- **Dividers:** animated three-line water sheets; the fill follows the middle line.
- **Contact:** `tel:+17326003447` everywhere; `sms:+17326003447?&body=…` pre-filled ("Hi Sean! I found Above All online and I'd like a free estimate for <service>. Address / town: … Best time to reach me: …"); `mailto:info@AboveAllTeam.com`. Phone sticky bar (Call | Text) shows once the hero buttons scroll away and hides at the closing buttons. Desktop buttons show the number.
- **Tunables** at the top of the main `<script>` (`CFG`): jet radius, regrow speed (0.0045), idle wand speed, droplet counts, seam speed/amplitude. One shared animation loop; panels and seams pause off screen; reduced motion gets a still frame with one clean stripe.

## Assumptions I made
- **Muse missed assets that were on their site.** aboveallprowash.com has the logo (`/images/logo.png`), an email (`info@AboveAllTeam.com`, in their header) and two before/after "projects" images. I used all of them. The before/after photos are assumed to be Sean's own work because they're published as his projects.
- **Left out on purpose:** their service photos (blue-shirt workers on roofs and gutters) look like stock. Their shrink-wrap "project" photo looks AI-generated (a model wearing an "Above All" shirt). Neither is used as proof.
- **Painting and vinyl flooring** exist on their site but are commented out of the HTML, so I treated them as discontinued and left them off. Pest control is the sister brand and stays off too (per Muse's note).
- **Soft washing** got its own row (it's its own service card on their site). The "gutters twice a year" and "walk the entire project… 100% satisfied" lines are paraphrased from their site.
- **Call is primary, Text secondary**: the brief says texts are unknown and their site says "Call anytime!" But every service row is a text link (it's the best demo of text-to-book), so confirm Sean takes texts.
- Hero meta line "Family owned · Forked River, NJ · Since 2019" comes from their site and flyer.
- Testimonials are labelled "Testimonial on aboveallprowash.com" because they have no platform, date or stars. Two painting-focused ones (Richard M, Andrew C) are left out.
- The paver before/after was removed on Ellie's request. The siding before/after is the one slider, but its two photos are from different angles, so the boards don't line up under the divider. A matched-angle pair from Sean would fix it.
- Shrink-wrap gallery photos came from images Ellie supplied (2026-10-08): a boat on a lift (autumn-leaf stickers removed by inpainting, then cropped), two porch-furniture shots from a promo graphic, and three panels from their flyer (boat, wave runner, patio set). The flyer panels look polished enough that they may be stock or AI. Confirm with Sean that they're his jobs before this goes live.
- The Facebook link is the group-member profile URL Ellie gave. It may only open fully for people logged into Facebook or in that group.
- **Type:** system font stack (your house style) instead of Impeccable's "self-host a display face" rule.
- **No Impeccable concept roll / seed key:** the world was chosen unattended from the list below, so the contract has no seed.
- Review round (Impeccable finish reviewer): applied crisper wash cut, mildew collecting under each board lip, wet (not foggy) sheen, fan-shaped jet, sky-on-light contrast token `--sky-ink`, removed the "Shrink-wrap season" eyebrow and the faux film stripes, "…" on trimmed quotes, desktop numbers on text buttons, close wash strip pre-cleaned as the payoff (no regrow there). Kept against its advice after checking their site: Caitlin G's review, "get it right the first time, every time", furniture washing, and the shrink-wrap item list (all on aboveallprowash.com).

## Placeholders and gaps
- No hours, prices or Google/Yelp reviews (none published). Nothing invented.
- No shrink-wrap photo of real work. The panel is type and material only.
- Only two real before/after pairs. More would fill the proof section and could go in under each service row on phones.

## Questions for the owner
- Do you take texts at 732-600-3447? (Every service row and the sticky bar text you.)
- Real shrink-wrap photos (boats, hot tubs, patio sets)? And more before/afters, especially roofs, driveways and green siding?
- Hours? Do you give estimates from a photo by text?
- Are painting and vinyl flooring still offered?
- Is there a Google Business listing to link reviews from?
- Is shrink wrapping booked by a cutoff date? (A real deadline would make the "Boats and equipment." section stronger.) Do you wrap cars, trailers or other vehicles too?

## Ideas not built (yours to pick)
- **Runner-up world: shrink film.** The whole page is wrapped in glossy film that creases and stretches under the finger, peeling back to reveal sections. Strong for the seasonal push, weaker for washing.
- Other worlds considered: rain off a clean gutter (water sheeting off a roofline), soft-wash foam on siding, driveway pavers revealed tile by tile, sky/"Above All" clouds.
- Reviewer ideas not built: before/after divider drawn as the hero's fan spray with droplets; photo frames in the world's own material (wet siding edge / water sheet overlapping a seam) instead of white-bordered rounded frames; drips sheeting down freshly washed boards.
- Wash-panel game: "Clean 80% and get…" (only if Sean offers a promo), or the grime spelling a hidden message ("Call Sean") once cleaned.
- Booking form page (`book.html`) that composes the same pre-filled text, with a copy fallback.
- Seasonal toggle: swap the hero to the shrink-wrap pitch in Oct–Nov, back to washing in spring.
- Quote by photo: a step that tells people what to photograph before texting.
- Service rows on phones could each get a small before/after once more pairs exist.

## Not verified
- Real-device touch (iOS Safari, Android Chrome, Facebook in-app browser). Only headless simulated touch/mouse sweeps were tested.
- The real SMS handoff with the pre-filled body on iOS and Android, including newline handling in the body.
- Frame rate on older phones (the wash panel is a canvas redrawn every frame at up to 1.5x DPR on phones).
