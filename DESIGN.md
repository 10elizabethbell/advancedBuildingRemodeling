---
name: Advanced Building and Remodeling Associates
description: A calm, banded window-installer page for Ocean County homeowners. Paper and bay-dusk navy, one dusk-amber fill, nothing moves.
colors:
  paper: "#f4f6fb"
  card: "#ffffff"
  ink: "#0f2440"
  body: "#26364a"
  soft: "#4a5868"
  navy: "#1f4670"
  deep: "#0f2440"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d7ea"
  amber: "#f2a65a"
  amber-2: "#f6bd80"
  amber-ink: "#8a4b0c"
  line: "rgba(15,36,64,.12)"
  field: "#e6ecf5"
  focus: "#1f4670"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(40px, 11.5vw, 96px)"
    fontWeight: 400
    lineHeight: 1.04
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(32px, 8vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "24px"
    fontWeight: 400
    lineHeight: 1.2
  title-sm:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "20px"
    fontWeight: 400
    lineHeight: 1.2
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.6
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(18px, 4.8vw, 20px)"
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.4
rounded:
  field: "10px"
  row: "20px"
  card: "24px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter: "20px"
  gutter-wide: "40px"
  stack-sm: "12px"
  stack-md: "16px"
  stack-lg: "28px"
  column-gap: "64px"
  band: "64px"
  band-wide: "96px"
components:
  button-primary:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.ink}"
    typography: "{typography.title-sm}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.amber-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.title-sm}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.title-sm}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  link-row:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    typography: "{typography.title-sm}"
    rounded: "{rounded.row}"
    padding: "14px 16px 14px 22px"
    height: "72px"
  service-row:
    backgroundColor: "rgba(255,255,255,.07)"
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    rounded: "{rounded.row}"
    padding: "14px 16px 14px 18px"
    height: "80px"
  form-card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "56px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "52px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.on-dark}"
  step-number:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.ink}"
    typography: "{typography.title-sm}"
    rounded: "{rounded.circle}"
    size: "48px"
  float-text:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "60px"
---

# Design System: Advanced Building and Remodeling Associates

## Overview

**Creative North Star: "The Calm Band"**

The page is a stack of full-width colour bands that alternate between off-white paper, bay-dusk navy and a deeper navy at night. Each band carries one idea, set large in Cal Sans with plenty of room around it, and a single warm dusk-amber tells the eye where to press. The world is built for a homeowner over 40 reading on a phone: 18px body at 1.6, 56px tap targets, high-contrast ink, and a page that holds still.

Density is low and the order is fixed: say who and where, prove the license, show the windows, ask for the estimate, give the number. Surfaces are flat colour; depth comes from the band change and from white cards sitting on paper, never from shadows (the one exception is the floating text circle, which has to sit above content). There are no photographs in this system; drawn line icons (2.2 to 2.6px strokes, round caps) in navy carry the imagery.

Motion exists in code (a letter bounce-in for the H1, a 12px fade-up below the fold) but ships switched off (`CONFIG.MOTION = false`). The resting state is the design.

**Key Characteristics:**
- Full-bleed bands: paper, navy, deep navy with a faint diagonal line texture.
- One warm accent, dusk amber, used as a fill; text on it is always deep ink.
- Cal Sans at weight 400 for every heading, button, label and number; system sans for reading.
- Soft, large radii: 24px cards, 20px rows, pill buttons and chips.
- Still by default; every hover is a colour change only.

## Colors

A cool two-navy system on blue-tinted paper, warmed by a single dusk amber.

### Primary
- **Dusk Amber** (amber): the one action colour. Fills primary buttons, step numbers, the floating text circle, list bullets, hovered arrow discs and the hero accent words on navy. It is a fill, not a text colour on light grounds.
- **Lit Amber** (amber-2): hover state of amber fills only.
- **Burnt Amber Ink** (amber-ink): amber when it must be text on paper (accent words in headings on light bands, header phone hover), 6.3:1 on paper.

### Secondary
- **Bay-Dusk Navy** (navy): hero and closing bands; icon colour on light grounds; caret colour; and, as focus, the hover/focus outline for form controls on light grounds.
- **Night Navy** (deep): the windows band and the footer, always with the diagonal line texture.

### Neutral
- **Blue Paper** (paper): page ground and light bands; also the confirmation panel inside the form.
- **Card White** (card): form card and link rows on paper.
- **Deep Ink** (ink): headings and strong text on light; text on every amber fill; selected chip fill. Same value as Night Navy by design.
- **Slate Body** (body): running text on light.
- **Soft Slate** (soft): secondary text, field hints, placeholders.
- **Field Mist** (field): input and chip fill, visible against the white card.
- **Hairline** (line): 1px dividers between list items on paper.
- **Pale Night** (on-dark) and **Mist on Night** (on-dark-soft): headings and running text on navy bands.
- **Signal Red** (error): field error border and message.

### Named Rules
**The Amber Is a Fill Rule.** Amber appears as a solid shape (button, disc, dot, circle) with deep ink on top. On paper, amber text switches to burnt amber ink; bright amber text is allowed only on navy grounds.

**The Two Focus Colours Rule.** On light bands focus is a 3px navy outline at 3px offset; on navy and night bands it switches to amber. Focus never uses the same colour as the fill it surrounds.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** system sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans at its single regular weight gives friendly, rounded, sign-painter confidence; the system body keeps long text native and easy on older eyes.

### Hierarchy
- **Display** (400, clamp(40px, 11.5vw, 96px), 1.04): the hero H1 only, max 14ch, balanced wrap.
- **Headline** (400, clamp(32px, 8vw, 48px), 1.08): one H2 per band.
- **Title** (400, 24px, 1.2): step titles, service rows, claim lines, the service-area H3.
- **Title Small** (400, 20px, 1 to 1.2): buttons, field labels and legends, link rows, footer name, step numbers.
- **Lede** (400, clamp(18px, 4.8vw, 20px), 1.5): the paragraph under a band headline, max 38ch; the hero promise at max 30ch.
- **Body** (400, 18px, 1.6): all running text and inputs. Never smaller for reading copy.
- **Body Small** (400, 16 to 17px, 1.35 to 1.5): field hints, error text, claim sub-lines, the composed message preview.

### Named Rules
**The Display Does the Talking Rule.** Anything a visitor taps or scans (buttons, labels, rows, phone numbers) is set in Cal Sans; only prose and form input use the system face.

**The Phone Number Rule.** Phone numbers are Cal Sans with tabular figures, word-spacing -0.15em, never wrapping inside the number.

## Layout

A single 1160px centred column with a 20px gutter (40px from 760px). Bands pad 64px top and bottom on phones, 96px from 760px. Phones get one stacked column; hero buttons stack full width and go side by side from 760px (min 240px each). From 1024px most bands split into two columns with a 64px column gap: copy on the left, the proof list, service rows or form on the right; the estimate heading column is sticky at 40px. Vertical rhythm inside bands uses 12, 16, 22 and 28px steps. A 380px breakpoint trims chip and row padding for the smallest phones. The footer reserves 100px bottom padding so the floating circle never covers its links.

## Elevation & Depth

Flat. Depth is tonal: a band change, a white card on paper, or a 7% white wash on navy. The texture on hero, night bands and footer is a repeating 135deg line (1px at 3.5% white every 23px), felt more than seen.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(8,24,46,.3)`): the floating text circle only, because it sits over moving content.

### Named Rules
**The No-Lift Hover Rule.** Hover never adds a shadow or moves an element. It changes a colour: a row's arrow disc turns amber, a field border turns navy, amber lightens.

## Shapes

Generous, soft and consistent. Cards 24px, rows 20px, fields 10px, buttons and chips full pill, and every small token (step numbers, arrow discs, bullets, the floating button) a perfect circle. Borders are rare: 2px transparent borders on buttons, fields and chips exist so state can colour them without layout shift; hairline dividers separate list items. Icons are outlined line drawings in a 24 or 40/48 viewBox, round joins.

## Components

### Buttons
Pill-shaped, tall and unmistakable.
- **Shape:** full pill (999px), min-height 56px, 0 26px padding, Cal Sans 20px, optional 20px leading icon at 10px gap.
- **Primary:** amber fill and border, deep ink text. One per view where possible.
- **Hover / Focus:** primary lightens to amber-2 (pointer devices only); press scales to 0.98; focus outline per The Two Focus Colours Rule. Inside the form the submit is full width and gets a 2px navy outline on hover and focus.
- **Ghost:** transparent with a 2px 70% pale border and pale text, on navy only; hover goes solid white border with a 10% white wash.
- **Line:** transparent with a 35% ink border and ink text, on light grounds, for secondary actions.

### Chips
- **Style:** field-mist pill, 52px tall, 18px body text in ink, 2px transparent border; a styled label over a visually hidden radio.
- **State:** hover shows a navy border; selected fills deep ink with pale text; keyboard focus gets the 3px navy outline.

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** card white on paper.
- **Shadow Strategy:** none (see Elevation).
- **Internal Padding:** clamp(20px, 5vw, 32px), children 22px apart.

### Inputs / Fields
- **Style:** field-mist fill, 2px transparent border, 10px radius, 56px min height (textarea 120px), 18px text, navy caret. Labels sit above in Cal Sans 20px with optional hints in 16px soft slate.
- **Focus:** border turns navy; no glow. Hover does the same on pointer devices.
- **Error:** red border plus a 16px red sentence beneath that says what to add and why.

### Navigation
There is no menu. The paper header holds the two-line wordmark (Cal Sans 22/26px over 13/14px system sub-line) on the left and the tap-to-call number with a navy phone icon on the right, min 64px tall (76px desktop). The footer carries plain text links, 44px tall, pale on night, amber on hover.

### Link and Service Rows
The signature list device. A full-width rounded row (20px), 72px tall on paper (white) or 80px on night (7% white), with an icon and Cal Sans label on the left and a 44px circular arrow disc on the right. Only the disc changes on hover and focus: it fills amber with ink arrow; focus adds the outline around the disc.

### Numbered Steps
Ordered lists with a 48px amber circle carrying the number in Cal Sans 20px, then a 24px Cal Sans title and a soft-slate line beneath.

### Floating Text Circle
One 60px amber circle with a chat icon, fixed 16px from the bottom-right safe area. It appears after the hero leaves view and hides while the form is on screen. Never a bottom bar.

## Do's and Don'ts

### Do:
- **Do** keep body copy at 18px/1.6 and every tap target at least 44px (buttons and fields 56px).
- **Do** alternate bands paper, navy, night; put the line texture only on navy-family grounds.
- **Do** put deep ink on amber, and switch amber text to burnt amber ink on paper.
- **Do** set headings, buttons, labels and phone numbers in Cal Sans 400.
- **Do** ship still: motion stays behind `CONFIG.MOTION` and off for this audience.

### Don't:
- **Don't** use amber as body or label text on light grounds.
- **Don't** add shadows to cards, rows or buttons; the floating circle is the only lifted element.
- **Don't** make hover move, lift or glow anything.
- **Don't** add a sticky bottom call bar; the single floating circle is the persistent action.
- **Don't** put an eyebrow pill on every heading. Ellie's calm style (2026-10-19) puts one above the hero H1 and a few key section headings only: 14px, an amber dot, a faint tint, no arrow, no hover, no shadow. Impeccable's craft floor bans eyebrows; this is Ellie's call.
- **Don't** use Cal Sans bold or a second display face; the system has one display weight.
