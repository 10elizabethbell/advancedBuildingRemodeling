---
name: Advanced Building and Remodeling Associates
description: A replacement-window pitch page you look through, not at. A fogged white vinyl window at dusk over the bay.
colors:
  wall: "#1a3049"
  wall-deep: "#132539"
  wall-soft: "#24405e"
  vinyl: "#f6f7f5"
  vinyl-2: "#e3e7e9"
  vinyl-shade: "#cbd2d8"
  vinyl-white: "#ffffff"
  ink: "#15283c"
  ink-soft: "#3e5266"
  on-wall: "#eef3f7"
  on-wall-soft: "#b9c9d7"
  amber: "#f2a65a"
  amber-hover: "#f6b673"
  amber-deep: "#d9823a"
  amber-pale: "#f8d3a8"
  amber-ink: "#9a5218"
  fog: "#dfe8ee"
  pane-glass: "#e6eef3"
  pane-glass-deep: "#d6e2ea"
  field-face: "#fbfcfd"
  field-line: "#c3cfd9"
  field-placeholder: "#5f7183"
  error: "#b23a2a"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.5rem, 6.4vw, 5.1rem)"
    fontWeight: 900
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2rem, 4.6vw, 3.4rem)"
    fontWeight: 900
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.5rem"
    fontWeight: 900
    lineHeight: 1.02
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.1rem"
    fontWeight: 400
    lineHeight: 1.55
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "0.92rem"
    fontWeight: 800
    lineHeight: 1.55
  button:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1rem"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "0.01em"
  credential:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "0.98rem"
    fontWeight: 900
    lineHeight: 1.15
    letterSpacing: "0.03em"
rounded:
  vinyl: "3px"
  pane: "4px"
  field: "10px"
  frame: "12px"
  card: "14px"
  pill: "999px"
spacing:
  gutter: "clamp(16px, 4vw, 48px)"
  container: "1180px"
  section-top: "clamp(56px, 8vw, 104px)"
  section-bottom: "clamp(80px, 10vw, 130px)"
  column-gap: "clamp(28px, 5vw, 64px)"
  mullion: "14px"
  field-gap: "16px"
  pair-gap: "12px"
  chip-gap: "8px"
components:
  button-primary:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 1.4em"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.amber-hover}"
    textColor: "{colors.ink}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.on-wall}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 1.4em"
    height: "56px"
  button-line-on-vinyl:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    height: "56px"
  field:
    backgroundColor: "{colors.field-face}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
  chip:
    backgroundColor: "{colors.field-face}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 16px"
    height: "44px"
  chip-selected:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
  stepper-button:
    backgroundColor: "{colors.field-face}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    size: "52px"
  type-row:
    backgroundColor: "#fdfdfc"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "16px 16px 16px 14px"
  lite-pane:
    backgroundColor: "{colors.pane-glass}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pane}"
    padding: "clamp(22px, 3vw, 34px)"
  vinyl-frame:
    backgroundColor: "{colors.vinyl}"
    rounded: "{rounded.frame}"
    padding: "{spacing.mullion}"
  credentials-strip:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.ink}"
    typography: "{typography.credential}"
    padding: "30px 0 64px"
  sticky-bar:
    backgroundColor: "{colors.wall-deep}"
    padding: "10px 16px"
---

# Design System: Advanced Building and Remodeling Associates

## Overview

**Creative North Star: "The Fogged Window at Dusk"**

The page is the installer's product. A navy wall at dusk holds white vinyl windows, and every content container is either a pane of glass in a vinyl frame or the wall around it. The hero is a working double-hung window: fogged condensation you wipe clear with a finger or cursor, beads that get shoved and spring back, heavy beads that run and leave a streak, and a dusk scene over the bay behind it. Amber is the light coming in off the bay, and it marks every action.

Density is low and direct, like a flyer: one heavy uppercase headline per section, one short lede, then something you can press. Sections alternate between the navy wall and the white vinyl ground. Animated water-line seams straddle each boundary, so you never see a hard edge between sections. Depth is physical. Frames cast long soft drop shadows onto the wall, and glass sits recessed under an inset shadow from the frame above it.

This system was recorded after an unattended, code-led build. The direction was unseeded: no concept-seed roll, fogged window chosen first of six worlds, with drafts-and-curtains as the runner-up. A finish review's eight material fixes were all applied before this record: real double-hung sash structure, white vinyl tokens, seams straddling section edges with shaded beads, `amber-ink` for amber text on light grounds, card icons removed from the four-lite panes, focus moved to the confirmation, and seams around the credentials strip. No raster assets ship. Every image is CSS, inline SVG, or canvas painted at runtime.

**Key Characteristics:**
- Dusk navy wall, white vinyl frames with soft bevel gradients, blue-white fogged glass, one amber light.
- Heavy uppercase system sans for headings; sentence case for body, buttons and labels.
- Content sits in panes: recessed glass inside vinyl frames, separated by a 14px mullion.
- Water-line seams with riding beads straddle every section boundary.
- One rAF loop for all motion. Motion pauses off-screen, and reduced motion gets a still, pre-wiped frame.

## Colors

The palette is a dusk window: cool navy and white-vinyl neutrals carry nearly everything, and a single warm amber is the light.

### Primary
- **Dusk Amber** (amber): the light off the bay. It fills every primary button, the selected chip, the type-row arrow disc, the seam's middle water line, the hero headline's second line, the focus ring, and the full-bleed credentials strip. On navy it reads as light; on vinyl it is a fill, never text.
- **Lit Amber** (amber-hover): the primary button's hover. It is one step lighter, as if the light came up.
- **Burnt Amber** (amber-deep): amber's edge color on light grounds. Used for line-button borders on vinyl, field and chip hover borders, the focused field border, map-pin icons on vinyl, and the text caret.
- **Amber Ink** (amber-ink): the only amber allowed as text on vinyl or other light grounds (the flyer line, "home base" sublabel). It exists because Dusk Amber fails contrast on white.
- **Amber Pale** (amber-pale): text selection highlight.

### Neutral
- **Dusk Navy Wall** (wall): the hero, estimate and close grounds, plus the page background and `theme-color`.
- **Deep Wall** (wall-deep): the sticky phone bar (at 94% with a 10px backdrop blur) and the scrollbar track.
- **Soft Wall** (wall-soft): step-number discs on navy, window-type icon strokes, and the scrollbar thumb.
- **White Vinyl** (vinyl), **Vinyl Bevel** (vinyl-2), **Vinyl White** (vinyl-white): the frame material. Light sections sit on White Vinyl. Frames, sashes, the meeting rail and the sill are 160-degree gradients running from Vinyl White through White Vinyl to Vinyl Bevel. The sash borders are solid Vinyl White.
- **Vinyl Shade** (vinyl-shade): hairline rules between town names on vinyl.
- **Navy Ink** (ink) / **Soft Ink** (ink-soft): text and secondary text on vinyl, glass and amber.
- **On-Wall** (on-wall) / **On-Wall Soft** (on-wall-soft): text and secondary text on navy.
- **Fog** (fog): the breath-on-glass tint, used for window-type icon fills and the fog canvas base.
- **Pane Glass** (pane-glass → pane-glass-deep): the 170-degree gradient of a recessed glass pane. The form pane uses a slightly lighter pair (#eef3f6 → #e1e9ef).
- **Field Face / Field Line / Field Placeholder**: the input surface, its 2px border, and placeholder text.
- **Error** (error): field border and message on the light form pane.

### Named Rules
**The Dusk Light Rule.** Amber is the only warm color and it means "act here" or "this is the light." Every primary action is amber, and no other hue is introduced for emphasis.

**The Amber Ink Rule.** Dusk Amber is never text on a light ground. Amber words on vinyl or glass use Amber Ink. Dusk Amber text appears only on the navy wall.

**The Two Grounds Rule.** Sections alternate wall and vinyl. The amber credentials strip is the single exception, and it is still bounded by seams on both sides.

## Typography

**Display Font:** system UI sans (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial)
**Body Font:** the same stack

**Character:** Flyer weight. Black (900) uppercase headings with tight leading do the shouting, and plain regular body copy does the explaining. The system stack is the owner's house style for this project and a deliberate choice, not a webfont fallback. It is scoped to this project and is not a default to carry into other worlds.

### Hierarchy
- **Display** (900, clamp(2.5rem, 6.4vw, 5.1rem), 1.02, uppercase): hero headline only. The second line is set in Dusk Amber.
- **Headline** (900, clamp(2rem, 4.6vw, 3.4rem), 1.02, uppercase): section headlines. The close headline runs larger (clamp(2rem, 5.6vw, 4.2rem), max 16ch) because it carries the business name.
- **Title** (900, 1.5rem, uppercase): pane and form headings. Window-type names use the same face at 1.12rem.
- **Lede** (400, 1.1rem, 1.55, max 52ch): the one paragraph under each headline, in Soft Ink or On-Wall Soft.
- **Body** (400, 17px, 1.55, ~40ch inside panes).
- **Label** (800, 0.92rem, sentence case): form labels and legends. Hints in parentheses drop to 600 in Soft Ink.
- **Button** (800, 1rem, 1, +0.01em, sentence case).
- **Credential** (900, 0.98rem, +0.03em, uppercase): credential items on the amber strip, each with a 0.78rem/700 sentence-case sub-line.

### Named Rules
**The Heavy Caps Rule.** Only headings, titles, the wordmark and credentials are 900 uppercase. Buttons, labels, ledes and body stay in sentence case at 800 or less, so the caps keep their punch.

**The Balanced Head Rule.** Headings use `text-wrap: balance` and paragraphs `text-wrap: pretty`. Long headlines break by hand (`<br>`) at the phrase, as in "New windows. / Installed sooner."

## Layout

A single centered column, max 1180px, with a fluid gutter (clamp(16px, 4vw, 48px)). Sections pad clamp(56px, 8vw, 104px) on top and clamp(80px, 10vw, 130px) on the bottom. The extra bottom room is where the next seam's 70px water line rises into the section.

Two-column splits are always slightly asymmetric and collapse to one column below the breakpoint. The text side comes first on phones.
- Hero: 1.05fr / 0.95fr at 900px (window right, below on phones).
- Window types and service area: 0.9fr / 1.1fr at 900px.
- Estimate: 0.85fr / 1.15fr at 960px.
- Four-lite panes: two columns at 760px.
- Form fields: two columns at 560px; address, type, count and notes span full width.
- Towns: CSS columns, 2 then 3 at 560px.
- Credentials: 2×2, then a single spaced row of 4 at 860px.

Button pairs flex-wrap with a 12px gap and a 220px basis, so they stack on narrow phones. Below 760px a fixed sticky bar (amber "Request an estimate" plus a 52px call button) keeps the estimate one thumb away. It slides out of the way while the hero buttons, the form, or the close buttons are on screen. The desktop top bar shows the phone number at 760px and up.

## Elevation & Depth

Depth is physical: a lit frame standing off a wall, glass recessed inside it. Frames cast long, soft, navy-tinted drop shadows downward onto the wall. Glass and panes sit under an inset shadow falling from the frame's top edge. No glows, no colored shadows, no hard offsets.

### Shadow Vocabulary
- **Frame drop** (`0 40px 70px -30px rgba(4,12,24,.8), 0 12px 24px -8px rgba(4,12,24,.45)`): a vinyl frame on the navy wall (hero window, form sash).
- **Lift** (`0 18px 40px -18px rgba(8,20,36,.55), 0 4px 10px rgba(8,20,36,.18)`): a vinyl frame on the vinyl ground (four-lite window).
- **Pane inset** (`inset 0 5px 10px -4px rgba(0,0,0,.27)`): every glass pane, including the form pane, under its frame.
- **Glass inset** (`inset 0 6px 12px -4px rgba(0,0,0,.38), inset 0 -2px 8px rgba(0,0,0,.16)`): the hero glass.
- **Sash** (`inset 0 5px 9px -3px rgba(0,0,0,.32), 0 2px 6px rgba(0,0,0,.2)`): the two sash borders.
- **Card rest / hover** (`0 10px 24px -16px rgba(8,20,36,.45), 0 2px 4px rgba(8,20,36,.06)`, deepening to `0 16px 30px -16px rgba(8,20,36,.5)` with a 2px rise): window-type rows.
- **Button** (`0 8px 18px -8px rgba(8,20,36,.5)`): amber buttons only.
- **Sill** (`0 16px 24px -10px rgba(4,12,24,.7)`): the sill under the hero window.

### Named Rules
**The Light From Above Rule.** Shadows fall down. Drop shadows have positive y-offsets and negative spread, and inset shadows come from the top edge. A shadow that points sideways or up is wrong.

## Shapes

Vinyl hardware is nearly square, and the things you touch are round. Frames and sashes use 3px corners, glass panes 4px, the framed form and four-lite window 12px, window-type rows 14px, and fields and stepper buttons 10px. Buttons, chips and the wipe hint are full pills (999px). Circles appear only as 40–44px discs (the type-row arrow, step numbers).

Bevel is carried by gradients, not borders. Vinyl is a 160-degree white-to-bevel gradient, glass a 170-degree pale-blue gradient. A **mullion** (14px) separates panes inside a frame and pads the frame around them. Lines appear as hairlines between town names, the footer rule, and the 2px field and line-button borders.

## Components

### Buttons
Round, warm, and big enough for a thumb.
- **Shape:** full pill (999px), minimum height 56px (52px in the sticky bar), padding 0 1.4em, 2px border, leading 22px line icon with a 0.55em gap.
- **Primary (amber):** Dusk Amber fill and border, Navy Ink text, button shadow. Hover lifts to Lit Amber.
- **Line (on wall):** transparent with an amber border and On-Wall text. Hover adds an amber wash (rgba(242,166,90,.14)).
- **Line (on light grounds):** Navy Ink text with a Burnt Amber border.
- **Press:** scale(.97) over 0.2s cubic-bezier(.2,.8,.2,1).
- **Focus:** a 3px Dusk Amber outline at a 3px offset, used globally.
- Buttons come in pairs (Text first, Call second), with a separate underlined text link to the form.

### Window frame and sash (signature)
The vinyl component language. Any container holding something important is a window.
- **Double-hung (hero):** a 3px-cornered vinyl frame with 20px of padding, frame drop shadow, over 4:5 glass. Two sash frames (9px solid Vinyl White borders, sash shadow), each 50% + 4px tall. The lower sash sits in front. A 28px meeting rail with a bevel gradient carries a 46×14px tan sash lock. A sill 18px tall overhangs the frame by 14px on each side.
- **Framed pane (form):** a 12px vinyl frame with 14px of padding and frame drop, holding a 4px glass pane (lighter glass gradient, pane inset, clamp(20px, 3.4vw, 34px) of padding).
- **Four-lite (reasons):** a 12px vinyl frame with 14px padding and a 14px mullion gap, lift shadow, holding four glass panes of title plus body. Panes hold words only, no icons.

### Fogged glass engine (signature)
Four stacked canvases inside the hero glass, bottom to top:
1. **Scene:** a dusk sky gradient (#2a4868 → #5a7290 → #d4936a → #f2b072 at a 44% horizon), a low sun glow at 64% across, a barrier-island silhouette (#1b3149), and the bay (#2f4a66 → #172c45) with drifting light streaks (warm #ffd29a near the horizon, cool #9fb7cc farther down).
2. **Blur:** a low-resolution copy of the scene, masked to the fog.
3. **Fog:** a mottled breath texture (base rgb(214,226,235), denser toward the bottom) at 0.34 resolution, CSS blur(3px) scale(1.03). Wiping erases it with `destination-out`, and it breathes back at a gently varying rate.
4. **Beads:** pre-rendered sprites (radii 1–9). Each has a filled shaded body (warm cream to steel blue to navy), a soft offset shadow, and one soft specular spot. They never use hairline glints.

Behavior: the pointer or finger wipes the glass and shoves nearby beads, which spring back with a wobble. A bead shoved past the break distance, or grown past the run radius, runs down, merges with beads in its path, and clears a streak. A ghost finger wipes a lazy S across the top sash at ~0.6s and again after idle, so the idea reads without instructions. A dark pill hint ("Wipe the glass", 78% Navy Ink) fades out at first real touch. Touch uses `touch-action: pan-y` and passive listeners so the page still scrolls. Before JS runs, the glass shows a static CSS gradient of dusk behind fog.

Tunable constants (the `C` object at the top of the engine): `FOG_SCALE` 0.34, `FOG_OPACITY` 0.74, `REFOG` 0.16/s, `WIPE_R` 30px, `DROPS` 80 (42 on phones), `PUSH_R` 52px, `BREAK` 13px, `SPRING` 38, `DAMP` 6.5, `GROW` 0.07px/s, `RUN_AT` 5.4px, `RUN_MAX` 150px/s, `GHOST_EVERY` 9s, `STREAKS` 44 (26 on phones). Tune behavior here, not in the step code.

### Seams (signature)
Animated water lines between every pair of sections, including both sides of the credentials strip. Each is an SVG 70px tall at full width, positioned `top: -69px` so it straddles the boundary. Its fill follows the middle line in the next section's color (`--next`). There are three sine-sum lines, all 2px non-scaling strokes: the back line at 30% fog, the front line at 55% fog, and the middle line in Dusk Amber. Going into a navy section, the fog lines switch to navy-blue at 45% and 28%. Three beads (radii 4, 5, 6.5) ride the middle line using a shared radial gradient (cream to steel to navy). A pointer passing within 30px raises a Gaussian swell under it that decays at a rate of 2.5/s. Constants: `STEP` 20, `SWELL` 9, `RIPPLE` 3.2, `SPEED` 1.5, `BUMP` 16. The same code drives every seam.

### Window-type rows
Each row is a whole-row link that preselects its type in the form. It has a 14px card shape, near-white fill, and card rest shadow, on a 56px / 1fr / 44px grid: a drawn line icon of the window type (Fog fill, Soft Wall stroke), a 900 uppercase name over a Soft Ink line, and a 40px Dusk Amber arrow disc. Hover lifts the row 2px and nudges the disc 3px right.

### Inputs / Fields
- **Style:** Field Face fill, 2px Field Line border, 10px corners, 13×14px padding, 500 weight at 1.02rem.
- **Focus:** the border shifts to Burnt Amber with a 4px amber ring (rgba(242,166,90,.3)). There is no outline.
- **Error:** the border goes Error, and a 700 0.88rem message appears below, announced politely. Focus jumps to the first bad field and the error clears on input.
- **Chips (window type):** single-choice radios styled as 44px pills with a Field Line border. Hover gives a Burnt Amber border. Selected is filled Dusk Amber. Keyboard focus is a 3px Burnt Amber outline.
- **Stepper:** 52px minus/plus buttons on either side of a centered, 800-weight tabular-number field. Native spinners are hidden.
- **Confirmation:** on submit the fields hide and a "Your text is ready" panel takes the pane. Focus moves to its heading. It shows the composed message in a field-styled block, an Open text / Copy message pair, and an underlined "Edit my details" link.

### Credentials strip
A full-bleed Dusk Amber band in Navy Ink with seams on both edges. It lists four credentials (28px line icon plus Credential type) and one sentence-case verification line with an 800-weight link.

### Navigation
There is no menu. The top bar holds the wordmark: a small drawn window mark (white frame, amber upper lite, navy lower lite with a fog band), "Advanced" in 900 uppercase, and the full legal name below in On-Wall Soft. A phone link sits at the right on 760px and up. On phones the sticky bar described in Layout replaces it.

### Icons
Inline SVG line icons on a 24px grid: 2px round-capped stroke in `currentColor`, 22px default size (18px in trust lines and the hint, 28px in credentials). They always sit next to words, never alone, except the sticky call button, which has an aria-label.

### Motion
- **One loop:** every animated task registers with the single shared rAF loop. The loop stops when no task is active and is kicked by input or visibility.
- **Pause off-screen:** each task is gated by an IntersectionObserver with an 80px margin.
- **Reduced motion:** no rAF at all. The fog draws once as a still frame with one horizontal wipe already cleared. The hint is hidden, seams draw their resting shape, and smooth scroll is turned off.
- **UI transitions:** ease cubic-bezier(.2,.8,.2,1). Fields 0.15s, buttons 0.2s, cards 0.25s, sticky bar 0.35s, hint fade 0.6s.

## Do's and Don'ts

### Do:
- **Do** put important content in a window: a vinyl frame (12px, 14px mullion) holding recessed glass panes (4px, pane inset).
- **Do** make every primary action a Dusk Amber pill at least 56px tall, paired with a line button for the other channel.
- **Do** use Amber Ink for any amber text on vinyl, glass or white.
- **Do** separate sections with a seam that straddles the edge and fills with the next section's color, including around the amber strip.
- **Do** register any new animation with the shared loop, gate it with `watchVisible`, give it a still reduced-motion frame, and expose its tunables in a `C` object.
- **Do** draw water as filled, shaded beads with one soft highlight.
- **Do** keep headings 900 uppercase and everything else sentence case.
- **Do** paint imagery in CSS, SVG or canvas. If real install photos arrive, they go inside vinyl frames as glass panes.

### Don't:
- **Don't** use the contractor template the thesis refuses: a stock house photo, a blue banner, or a grid of service cards.
- **Don't** set Dusk Amber text on a light ground, or introduce a second accent hue.
- **Don't** put icons inside the four-lite glass panes. Panes hold words.
- **Don't** draw a double-hung window without both sashes, the meeting rail and its lock. A single framed rectangle is not this product.
- **Don't** start a second requestAnimationFrame loop or animate anything while it is off-screen.
- **Don't** draw beads as hairline glints or outline rings.
- **Don't** use hard offset shadows, glows or sideways shadows. Light comes from above.
- **Don't** let a seam sit entirely inside one section or end in a straight edge.
- **Don't** add a small uppercase label above a headline. Section openings start with the headline itself.
