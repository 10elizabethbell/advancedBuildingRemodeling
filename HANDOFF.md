# Advanced Building and Remodeling Associates — handoff at ~60%

**Live:** https://10elizabethbell.github.io/advancedBuildingRemodeling/ · **Repo:** https://github.com/10elizabethbell/advancedBuildingRemodeling (public) · **Built:** 2026-10-08 from the Muse brief of 2026-10-08 · **Revamped:** 2026-10-19 to the calm band style

## Revamp, 2026-10-19: what changed
- **The whole page was rebuilt** from the DPG reference build (`~/Projects/freelance/dpgHomeImprovement/index.html`), in the calm band style (`calm-photo-style.md`).
- **The fogged-window world is gone.** That meant:
  - the wipe-to-clear hero canvas, the water-bead seams between sections, and the ghost finger
  - the amber credentials strip
  - the window-count stepper
  - it is all in git history at `d138df6` if you want any of it back
- **The page is a 40+ build now (inferred).** Ocean County replacement-window buyers are homeowners, and the county has many retirement communities, but the brief doesn't state an age. So nothing moves:
  - The H1 bounce-in and the fade-up are written but switched off (`CONFIG.MOTION = false` at the top of the script). Set it to `true` to turn both on; I tested that path and it works.
  - Body text is 18px at 1.6 line height.
  - Buttons are 56px.
  - Headings are sentence case.
  - The page is short: hero, trust, windows, estimate, close, footer.
- **Page weight:** 61KB of canvas code became a 27KB page with no images. The only external request is Cal Sans.
- **New files:** `favicon.svg` (a heavy "A" with an amber bar, on navy), plus a re-rendered `apple-touch-icon.png` and `og.png` (the new hero).
- **DESIGN.md and `.impeccable/design.json`** were regenerated from the new page. **PRODUCT.md** was updated (form fields, inferred audience age).

## What's built
- **Palette, mapped onto the calm style.** There is no logo and there are no brand colours, so I kept the old site's dusk palette:
  - paper `#f4f6fb`
  - bay-dusk navy `#1f4670` (hero, window rows, close)
  - deep navy `#0f2440` with the faint line texture (window types, footer)
  - dusk amber `#f2a65a`, used only as a fill with navy text on it
  - `#8a4b0c` when amber has to be text on light
  - the form hover/focus outline is navy
- **Header:** the "Advanced" wordmark plus "Building and Remodeling Associates" on the left, and the tap-to-call (609) 384-9030 in the top-right corner.
- **Hero:** a plain textured navy band. It has the eyebrow "Licensed, insured and bonded", the H1 "New windows in Ocean County, *installed sooner.*", "Ask for Joseph Carlucci. We make house calls.", and two buttons: Get an estimate (amber, jumps to the form) and Text Joseph (outlined, `sms:` with a pre-written body). There's no Call button.
- **Trust (paper):** "Check us out before we come over." It lists the NJ license #13VH10689900, insured and bonded, and the BuildZoom score 94 (top 24%, license verified Sept 2026). Under that are two rows, See more on Facebook and See us on BuildZoom; only their arrow changes on hover.
- **Windows (deep navy):** an eyebrow, "The windows we put in.", four short facts from the flyer, and three rows (Double, Picture, Bay). Each row jumps to the form and pre-selects that window type.
- **Estimate (paper):** three static steps beside the form.
  - Required fields: name, street and town.
  - Optional fields: window type chips, how many, notes.
  - Submit writes one text to Joseph. If the messages app doesn't open, a panel shows the message with Open in Messages, Copy, and the number to call. There's also a `<noscript>` fallback line.
- **Close (navy):** the business name, "Ask for Joseph Carlucci. Based in Manahawkin…", the big tap-to-call number, and all 33 Ocean County towns as plain text.
- **Footer (deep navy):** the name, Joseph, Manahawkin NJ, the phone, the license, and links to Facebook and BuildZoom. There's no email; the brief has none.
- **Floating text circle:** on. It shows after the hero, hides while the form is on screen, and gets `tabIndex=-1` and `aria-hidden` while hidden.

## Assumptions I made
- **The audience is 40+** (see above). That is the biggest call in this revamp. If you disagree, flip `CONFIG.MOTION`.
- **I didn't keep the old hero as a still picture.** older-audience.md says Ellie preferred her original hero made still over a new calm one. The revamp instruction was to adopt the calm style end to end, so I replaced it rather than freezing the fogged window. A still fogged window could come back as hero art if you want it.
- **The footer shows "Manahawkin, NJ", not "519 Shark Ln".** BuildZoom publishes the street address, but for a business that makes house calls it's probably Joseph's home. Put it back if he wants it shown.
- **The colours are mine** (no logo or flyer colours on hand).
- **The trust copy is mine:** "Check us out before we come over." and the "letting us into your home" line. The facts in it come from the brief.
- **The step copy is mine.** "He looks at the windows with you" is inferred from "We make House Calls."
- **"Installed sooner" and "no long wait"** come from the flyer's "IN STOCK & INSTALLED SOONER!". No timeline is promised.
- **The town list** is Ocean County's 33 municipalities. It's geography, not from the brief, and Stafford is labeled as Manahawkin.
- **I used "we" for the voice** ("Associates", with Joseph named as the contact).
- **No "free" anywhere,** because the brief never says the estimate is free.

## Placeholders and gaps
- **Every contact path except the phone number is SMS** (Text Joseph, the floating circle, the form), but the brief says "Accepts texts: unknown". If (609) 384-9030 is a landline, change the hero's second button and the circle to `tel:`, and make the form say "call to read it over".
- **There is no email,** so the footer has none.
- **The Facebook link goes to Joseph's personal profile,** which Muse couldn't view. A business page would be better.
- **The BuildZoom figures** (score 94, verified Sept 2026) will go stale. Re-check them before showing Joseph.
- **Missing:** a logo, work photos, before/afters, reviews, hours, prices and years in business. With real photos, the hero can become the calm style's photo-under-navy version, and a work-photo grid can go above the Facebook row.
- **Private history:** `brief.md` (Muse's prospecting notes) is still readable in the public repo's first commit, `e42f3dc`. The repo was already public before this session. Removing it means rewriting history and force-pushing, which I didn't do unattended. Your call before Joseph sees the repo.

## Questions for the owner
1. Does (609) 384-9030 take texts? If not, what's the best way to get a written request?
2. Are estimates free? Should the page say so?
3. Can you send a logo, 3+ photos of installs, and any before/after pairs?
4. What does "Lifetime Performance" cover (warranty wording)? Which window brands do you install?
5. Hours? How soon is "installed sooner" in practice?
6. Is it OK to show 519 Shark Ln on the site? Any towns you'd rather not take?

## Ideas not built (yours to pick)
- **Impeccable findings I kept against its advice (your calm-style choices):**
  - The eyebrow pills: three of them (hero, windows, estimate). The craft floor bans eyebrows outright.
  - The diagonal band texture: the detector flags `repeating-stripes-gradient`. I added a narrow ignore for it in `.impeccable/config.json` with the reason recorded.
  - The detector's `flat-type-hierarchy` note covers body sizes only (14–24px). Headings run 32–96px, so I left it.
- **Font to try for this audience:** Atkinson Hyperlegible for body text (older-audience.md).
- **Runner-up world (opt-in signature motion):** the old fogged window, drawn once as a still picture in the hero (no wiping). For a younger audience it could be the original wipe-to-clear glass, or drafts and curtains (a sheer curtain that stills once the new windows are in).
- **Calm-style pieces with no material yet:** work photo cards (4:5, bottom gradient) and before/after sliders, once photos exist.
- **Copy alternatives:** use the flyer's "NEED NEW WINDOWS?" as the close headline, or "Affordable windows, installed sooner." as the H1. I left out "Affordable" because it reads as a price claim.
- The desktop hero's right half is plain navy (same as DPG). A real install photo would fill it.

## Not verified
- The real SMS handoff on iOS and Android (`sms:+1…?&body=`), and Copy inside Facebook's in-app browser.
- Real-device checks. Automated checks passed in Playwright Chromium and WebKit at 360, 390, 430, 844 and 1440px:
  - no sideways overflow
  - the primary button is in the first screen
  - inputs are 18px
  - the form errors and composed text are right
  - the floating circle states are right
  - the `sms:` bodies decode correctly
- Contrast was checked from the tokens, not by sampling pixels. The amber on navy accent is about 4.9:1, and it's only used at H1 size.
