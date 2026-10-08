# Advanced Building and Remodeling Associates — handoff at ~60%

**Live file:** index.html · **Repo:** https://github.com/10elizabethbell/advancedBuildingRemodeling (private) · **Built:** 2026-10-08 from the Muse brief of 2026-10-08 (revised mid-build; page follows the revised `brief.md`)

## What's built
- **World: fogged window glass.** The hero is a white vinyl double-hung window at dusk over the bay, fogged with condensation. Mouse or finger wipes it clear, and the fog slowly comes back. Beads of water get shoved by the pointer and spring back with a wobble. Shove one hard enough and it breaks free and runs down, clearing a streak. Heavy beads run on their own. A ghost finger wipes an S across the glass at load (and again after ~9s idle until someone touches it), so the idea reads without instructions.
- **Seams:** animated water lines between sections (three layered sine lines, the fill follows the middle line, beads ride it, and a pointer passing over raises a swell). Same code for every seam.
- **Sections:**
  - Hero: "New windows. Installed sooner." plus a pitch line, Text/Call pair, a link to the form, and a trust line.
  - Window types: double, picture and bay. Each whole row is a link that jumps to the form with that type preselected.
  - Why vinyl / Energy Star: four panes inside a four-lite window frame.
  - Estimate form.
  - Amber credentials strip, with the license # and BuildZoom line.
  - All 33 Ocean County municipalities.
  - Close with the business name, and a footer.
- **Contact:** every call link is `tel:+16093849030`, every text link is `sms:+16093849030`. The form (name, phone, address required; type chips; window-count stepper; notes) composes one text and opens it. A fallback panel shows the message with Open text / Copy and an Edit link. The sticky phone bar hides while the hero buttons, the form or the close buttons are on screen.
- **Motion budget:** one rAF loop. Each motion task pauses off-screen via IntersectionObserver. Reduced motion draws a still, pre-wiped frame. Phones get 42 beads instead of 80. Tunable constants are in the `C` object at the top of each IIFE.

- **Phone first (taste §0):** the page is designed at 360–430px and adapted up for desktop. On phones the fogged window sits right under the Text/Call buttons, with a square glass and the wipe hint in the top sash. The sticky bar opens a prefilled text. There are no new-tab links, every tap target is 44px+, secondary text is 14px+, and nothing scrolls sideways at 360/390.
- **Repo visibility:** private (created before the public-repo rule; left as is). `brief.md` IS committed; `src-assets/` is gitignored and empty.

## Assumptions I made
- **No "free" anywhere.** The first brief said "Request a free estimate"; the revised brief and the flyer never say the estimate is free, so I removed it. Restore it if Joseph confirms.
- **Hero headline** "New windows. Installed sooner." comes from his flyer ("IN STOCK & INSTALLED SOONER!", "GET NEW WINDOWS FASTER!"). The first version, "Clear glass. Warm rooms.", tied tighter to the fog world. Swap back if you prefer it.
- **The business name** is in the top-bar wordmark and the close headline, not the hero H1. This follows the house rule (benefit headline first). The first brief asked for the name in the hero.
- **Colors are mine:** dusk navy wall, white vinyl, amber dusk light. There are no known brand colors and no logo file; the wordmark plus a small drawn window mark stand in.
- **Window-type descriptions** are generic ("Two sashes that slide up and down…"). They aren't his words. "The everyday window in most Shore homes" is my inference.
- **Benefit copy** is general vinyl/Energy Star truth, with no numbers or savings percentages.
- **The town list** is Ocean County's 33 municipalities. Stafford is marked as home base, because Manahawkin is in Stafford Township.
- **"Joseph comes to you"** step: built from "We make House Calls." The "set a time to see your windows" part is inferred.
- **BuildZoom line** ("score 94, top 24% of NJ contractors", license verified Sept 2026) is quoted from the brief. It will go stale; re-check before showing him.

## Placeholders and gaps
- **Whether (609) 384-9030 takes texts is unknown.** The form and the hero's primary button depend on it. If it's a landline, switch the primary action to Call and make the form show the message plus "call to read it over" (or add an email).
- No logo file. The flyer image needs a logged-in Facebook browser, so it wasn't collected; its colors could replace mine.
- No work photos, before/afters, reviews, hours, prices, years in business, ZIP code.

## Questions for the owner
1. Does your cell take texts? If not, what's the best way to receive a written request (email)?
2. Are estimates free? Should the page say so?
3. Can you send a logo file, plus 3+ photos of installs (and any before/after pairs)?
4. Which brands or lines do you install, and what does "Lifetime Performance" cover (warranty wording)?
5. Hours, and how fast is "installed sooner" in practice?
6. Any towns or jobs you'd rather not take? (The page says every Ocean County town.)

## Ideas not built (yours to pick)
- **Runner-up world: drafts and curtains.** A sheer curtain billowing in a draft that the pointer pushes, and that goes still once "new windows" are in. Other candidates I listed: light rays through mullions, a thermal-camera heat-leak view, a measuring-tape/blueprint world, the bay seen through panes.
- **Phone number written in the fog** in the close section, as if finger-traced on a fogged pane, slowly fogging over and rewriting.
- Panes in the Why section that start fogged and clear as they scroll in, or on hover.
- Before/after sliders inside window frames once real photos exist.
- Window-type rows could show a small live fogged pane of that type on hover (desktop) instead of the static icon.
- Use the flyer's own all-caps lines more loudly, e.g. "NEED NEW WINDOWS?" as the close headline.

- **Tidy-up:** DESIGN.md records fewer values than the page uses: one-off small type sizes (.78–.88rem, 1.15rem, 1.25rem, 4.2rem), 6px/7px radii, sash-lock hardware colors and the pre-JS fallback gradient. I added narrow detector ignores for them in `.impeccable/config.json`. Folding them into the ramp, or adding them to DESIGN.md, is your call.

## Not verified
- Real-device touch: wiping with a finger while the page scrolls (listeners are passive and `touch-action: pan-y`), and iOS Safari canvas performance.
- The real SMS handoff on iOS and Android (`sms:+1…?&body=` format), and the Copy fallback on iOS.
- Frame rate on older phones: the fog does a 5-frame `getImageData` readback on a ~150×190 canvas plus three canvas layers with a CSS blur.
- Headless capture only: the stair-stepped wipe edge I saw headlessly is covered by a 3px CSS blur; check it on a real GPU.
