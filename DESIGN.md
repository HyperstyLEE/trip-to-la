---
name: SoCal Family Road Trip 2026
description: A sunny, editorial bilingual roadbook for an 8-day Southern California family drive
colors:
  sun: "#ff8c42"
  sun-deep: "#f2660a"
  amber: "#f6b13c"
  leaf: "#4c9a6b"
  leaf-deep: "#2f7350"
  ink: "#2a2018"
  ink-soft: "#6b5d50"
  paper: "#fff8ef"
  card: "#ffffff"
  line: "#efe3d2"
  xhs-red: "#ff2e51"
  xhs-red-deep: "#d11e3f"
  # Golden-hour sky (Three.js atmosphere gradient stops — extensions of the sunset identity)
  sky-hi: "#ffd28a"
  sky-mid: "#ff9e4d"
  sky-low: "#b8430a"
  # Night-drive sky (dark-theme atmosphere stops)
  night-hi: "#3a2a4d"
  night-mid: "#2a1d33"
  night-low: "#0d0a07"
typography:
  display:
    fontFamily: "Playfair Display, 'Noto Sans SC', Georgia, serif"
    fontSize: "clamp(2.4rem, 7vw, 4.6rem)"
    fontWeight: 900
    lineHeight: 1.04
    letterSpacing: "normal"
  headline:
    fontFamily: "Playfair Display, 'Noto Sans SC', serif"
    fontSize: "clamp(1.7rem, 4vw, 2.5rem)"
    fontWeight: 800
    lineHeight: 1.1
  title:
    fontFamily: "Playfair Display, 'Noto Sans SC', serif"
    fontSize: "1.12rem"
    fontWeight: 700
    lineHeight: 1.3
  body:
    fontFamily: "'Work Sans', 'Noto Sans SC', system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "'Work Sans', sans-serif"
    fontSize: "0.76rem"
    fontWeight: 700
    letterSpacing: "2px"
  mono:
    fontFamily: "'Spline Sans Mono', 'Noto Sans SC', ui-monospace, monospace"
    fontSize: "0.8rem"
    fontWeight: 500
    letterSpacing: "-0.01em"
    note: "Telemetry layer — clock times, mileage, coordinates, prices, charge stats, romanized English subtitles. The trip's co-driver logbook voice; never long-form prose."
rounded:
  sm: "6px"
  md: "12px"
  lg: "16px"
  xl: "20px"
  page: "26px"
  pill: "999px"
spacing:
  xs: "6px"
  sm: "10px"
  md: "16px"
  lg: "22px"
  xl: "56px"
components:
  button-primary:
    backgroundColor: "{colors.leaf-deep}"
    textColor: "{colors.card}"
    rounded: "{rounded.pill}"
    padding: "6px 11px"
  button-cta:
    backgroundColor: "{colors.sun}"
    textColor: "{colors.card}"
    rounded: "{rounded.pill}"
    padding: "12px 22px"
  chip:
    backgroundColor: "{colors.line}"
    textColor: "{colors.ink-soft}"
    rounded: "{rounded.pill}"
    padding: "3px 9px"
  xhs-link:
    backgroundColor: "{colors.xhs-red}"
    textColor: "{colors.card}"
    rounded: "{rounded.pill}"
    padding: "6px 11px"
  card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    rounded: "{rounded.lg}"
    padding: "16px 17px"
---

# Design System: SoCal Family Road Trip 2026

## 1. Overview

**Creative North Star: "The Golden-Hour Roadbook"**

This is a keepsake travel journal lit by California's late-afternoon sun, not a booking
portal and not a feed. It carries an editorial spine — a serif display voice, generous
column rhythm, considered color — wrapped around genuinely useful trip logistics. The
feeling on open should be the warm tilt of light at 6pm on the Pacific Coast Highway:
anticipation, ease, the sense that the trip has already begun. It is a private companion
for one family, so it earns the right to be specific, warm, and a little playful (palm
fronds, a countdown, golden gradients) rather than generic and "safe."

The whole surface rides a committed warm-neutral paper (`#fff8ef`) with a single sunset
gradient carrying the hero and primary actions. Warmth is the brand's native climate; the
green (`--leaf`) is the orange's counterweight — used for "go" actions, kid notes, and
confirmation, never decoratively. 小红书 red (`#ff2e51`) is a strictly-scoped third voice
that means exactly one thing: "this is a real reference you can open." Density is editorial-
medium: each section answers its question at a glance, with detail tucked into expandable
day cards and an image lightbox rather than crammed onto the page.

This system explicitly rejects three things, carried verbatim from PRODUCT.md: the **generic
travel-agency template** (stock heroes, "deals" framing, corporate blue), the **cluttered
小红书 screenshot-collage** (emoji-soup as layout, unscannable card walls), and the **cold
SaaS dashboard** (sterile chrome, gray-on-white, zero personality).

**Key Characteristics:**
- Warm paper surface + a single sunset gradient as the signature, not a flat white app shell.
- Serif display (Playfair) against humanist sans (Work Sans) — real contrast, one bilingual voice.
- Green = action/confirm, orange = identity/warmth, 小红书 red = "open a real source."
- Glanceable first: collapsible day cards, an image lightbox, lazy-loaded detail.
- Dual-theme, built for bright sun and night-driving alike.

## 2. Colors

A sunset-over-the-coast palette: warm citrus and amber against eucalyptus green, grounded
on soft warm paper.

### Primary
- **Coast Sunset Orange** (`#ff8c42`, deep `#f2660a`): The brand's signature. Carries the
  hero gradient, the primary CTA buttons (planner "generate", map "navigate"), active plan
  tabs, day-number accents, and links (`--sun-deep` for sufficient contrast on paper).
- **Golden Amber** (`#f6b13c`): The warm highlight. Price tags, day badges, the packing
  progress bar's leading edge, hero glow. The lighter, friendlier partner to the orange.

### Secondary
- **Eucalyptus Green** (`#4c9a6b`, deep `#2f7350`): The action/affirmation voice. Primary
  "navigate" pills, kid-friendly notes, completed checklist items, recommended-plan flag.
  Its job is "go" and "good" — never decoration.

### Tertiary
- **小红书 Red** (`#ff2e51`, deep `#d11e3f`): Reserved exclusively for real reference links
  (小红书 cards, source buttons, café/vlog markers). When you see red, you can open a source.

### Neutral
- **Warm Ink** (`#2a2018`): Primary body and heading text. A warm near-black, never pure
  `#000`.
- **Soft Ink** (`#6b5d50`): Secondary/meta text and English subtitles. Watch contrast — see
  the Reading-Floor Rule.
- **Coastal Paper** (`#fff8ef`): The body surface. A committed warm off-white, the brand's
  climate.
- **Card White** (`#ffffff`): Raised surfaces lift off the paper by being cleaner/cooler.
- **Sand Line** (`#efe3d2`): Hairline borders, dividers, dashed separators, unselected chips.

### Dark Theme
Paper inverts to warm near-black (`#17120d`), cards to `#211a13`, ink to warm cream
(`#f3e9db`), soft ink to `#b9a892`, lines to `#34291d`. The sunset gradient and red/green
accents carry across unchanged — the identity holds in both lights.

### Named Rules
**The One-Job-Per-Color Rule.** Green means action/confirm. Red means "open a real source."
Orange means identity and warmth. A color never borrows another's job; that discipline is
what keeps a warm, saturated palette from reading as 小红书 emoji-soup.

**The Reading-Floor Rule.** Body and meta text must clear 4.5:1 against their actual
background in **both** themes. `--ink-soft` (`#6b5d50`) on paper is the one to verify
constantly; if a passage is long-form reading rather than a one-word label, push it toward
`--ink`. Light gray "for elegance" is forbidden.

## 3. Typography

**Display Font:** Playfair Display (with 'Noto Sans SC', Georgia, serif fallback)
**Body Font:** Work Sans (with 'Noto Sans SC', system-ui fallback)
**CJK Font:** Noto Sans SC carries all Chinese glyphs in both roles.

**Character:** A high-contrast serif display against a clean humanist sans — a true
contrast-axis pairing, editorial and warm without tipping into stuffy. Playfair's
sparkle gives the keepsake-journal feel; Work Sans keeps the logistics legible and modern.
中文 and English are one designed system: Chinese leads in Playfair/Work Sans weight, English
rides beneath as a lighter `--ink-soft` subtitle.

### Hierarchy
- **Display** (Playfair 900, `clamp(2.4rem, 7vw, 4.6rem)`, lh 1.04): Hero headline only.
  The italic 500-weight "scriptline" English subtitle is a signature flourish.
- **Headline** (Playfair 800, `clamp(1.7rem, 4vw, 2.5rem)`): Section titles (`h2`).
- **Title** (Playfair/Work Sans 700, ~1.12rem): Day titles, card headings (`h3`/`h4`).
- **Body** (Work Sans 400, 1rem, lh 1.6): Notes, descriptions, list items. Cap measure at
  65–75ch.
- **Label** (Work Sans 700, 0.76rem, +2px tracking, uppercase): Kickers, badges, meta tags.

### Named Rules
**The Bilingual Pair Rule.** Every place name appears as 中文 (primary weight) + English
(lighter `--ink-soft` subtitle) as one unit — never one language alone, never two competing
at equal weight.

**The One-Kicker Rule.** The uppercase tracked label is a deliberate accent, not section
scaffolding. Do not stamp an eyebrow above every section; let section rhythm and the serif
headlines carry the structure.

## 4. Elevation

A soft, lifted system: cards rest on warm diffuse shadows and rise on hover. Depth is
ambient (sunlit, not hard-edged) — shadows are tinted with the brand's brown, never neutral
gray or black, so they read as warm light rather than UI chrome.

### Shadow Vocabulary
- **Resting** (`box-shadow: 0 10px 30px -12px rgba(120, 72, 20, .28)`): Default card lift.
- **Lifted** (`box-shadow: 0 24px 60px -20px rgba(120, 72, 20, .38)`): Hover / featured /
  modal surfaces.
- **Dark theme** swaps the brown tint for `rgba(0,0,0,.6)`–`.7` since the surface is already dark.

### Named Rules
**The Warm-Shadow Rule.** Shadows are tinted with the paper's own brown hue, never neutral
gray/black. A gray shadow on warm paper is the tell that an element was dropped in from a
generic UI kit.

## 5. Components

### Buttons
- **Shape:** Fully pill (999px) for actions; CTAs and nav pills alike.
- **Navigate (primary action):** Eucalyptus gradient (`--leaf-deep → --leaf`), white text,
  small pill. Hover lifts 2px with a green-tinted shadow.
- **Generate / Map CTA:** Sunset gradient (`--sun → --sun-deep`), white text, larger pad.
- **Hover / Focus:** `translateY(-2px)` + colored shadow. Focus must show a visible ring
  (add `:focus-visible` outline — current build relies on hover only).

### Chips & Badges
- **Meta chip:** Sand-line background, soft-ink text, pill. Used for cuisine/area tags.
- **Price chip:** Amber-tinted background, deep-orange text.
- **Heat badge:** `hot` = warm peach bg / deep-orange text (🔥 爆款); `gem` = mint bg /
  deep-green text (⭐ 小众). Never rely on color alone — the emoji + label carry the meaning.

### Cards / Containers
- **Corner Style:** 16px (`lg`) for content cards, 20px (`xl`) for plan tabs / feature panels.
- **Background:** Card white on paper; hover lifts with `translateY(-4px)` + Lifted shadow.
- **Border:** 1px Sand Line. Plan tabs use 1.5px, switching to orange when active.
- **Internal Padding:** 16–17px cards, 18–24px panels.

### Navigation
- Sticky translucent paper bar with 12px backdrop blur and a Sand-Line bottom hairline.
- Pill links, soft-ink default → ink + sand-line bg on hover. Brand wordmark in Playfair 900.
- Mobile: link row is hidden under 560px (consider a compact menu affordance).

### Day Timeline Card (signature)
Expandable day card: a clickable header (day number, bilingual title, badge, chevron) over a
`max-height`-animated body of time-stamped segments. Plan A/B/C switching re-renders days
4–7 with a flash highlight. **Note:** the header currently uses a `border-left: 5px` accent
stripe — a banned side-stripe; replace with a full treatment (leading day-number block or
full top border).

### Image Lightbox (signature, 大图鉴赏)
Full-bleed overlay for large-image appreciation: rendered via native `<dialog>` / fixed
positioning to escape the timeline's `overflow:hidden` stacking context. Keyboard (←/→/Esc)
and swipe navigation, caption with place name + 小红书 source link, focus trap, and a
reduced-motion crossfade fallback.

## 6. Do's and Don'ts

### Do:
- **Do** keep the warm paper (`#fff8ef`) + single sunset gradient as the signature surface;
  it is the committed brand identity.
- **Do** tint every shadow with the brown paper hue (the Warm-Shadow Rule).
- **Do** keep green for action/confirm, red for "open a real source," orange for identity
  (the One-Job-Per-Color Rule).
- **Do** pair every place name 中文 + English as one unit (the Bilingual Pair Rule).
- **Do** verify `--ink-soft` body text clears 4.5:1 in both themes (the Reading-Floor Rule).
- **Do** add visible `:focus-visible` rings and respect `prefers-reduced-motion` on the
  countdown, reveals, card lifts, and lightbox.

### Don't:
- **Don't** let it read as a **generic travel-agency template** — no stock-photo heroes, no
  "deals" framing, no corporate blue.
- **Don't** let it become a **cluttered 小红书 screenshot-collage** — emoji are accents, not
  layout; keep card walls scannable.
- **Don't** drift toward a **cold SaaS dashboard** — no sterile gray-on-white chrome, no
  personality-free panels.
- **Don't** use a `border-left`/`border-right` greater than 1px as a colored accent stripe
  (the day-card stripe is being removed for exactly this reason).
- **Don't** stamp an uppercase tracked eyebrow above every section (the One-Kicker Rule).
- **Don't** use gradient text (`background-clip: text`), glassmorphism as default decoration,
  or gray shadows on the warm surface.

## 7. Motion & Atmosphere — "The Roadbook over a Living Horizon"

The site rides on a cinematic layer that deepens the golden-hour identity without
compromising legibility. Three commitments:

- **Living sky (Three.js).** A fixed full-viewport WebGL `ShaderMaterial` renders the
  golden-hour atmosphere — fbm-noise texture + film grain + a sun glow that follows the
  pointer (lerped). It is the brand's hero "imagery" (a credible WebGL scene, not a stock
  photo — honoring the no-stock-hero anti-reference). Theme-aware (`sky-*` light /
  `night-*` dark). It **pauses** on hidden tab and renders a single static frame under
  `prefers-reduced-motion`. The CSS `--sky` gradient is the no-WebGL fallback.
- **Roadbook pages.** Content sections are centered max-width paper "pages" that float
  over the fixed sky (the atmosphere shows in the desktop gutters and the gaps between
  pages). **Body text never sits on the live sky** — only the hero and the two full-bleed
  `.scene` chapter bands place cream type over it, always behind a contrast scrim.
- **Choreography (GSAP ScrollTrigger + Lenis).** Lenis drives smooth scroll; each section
  earns a *tailored* entrance (headline clip-reveals, batched card staggers, pinned scene
  captions, a fixed scroll odometer) — never one uniform fade on everything. Reveals
  **enhance an already-visible default**: the from-state is set by JS at runtime, so if
  scripts fail or motion is reduced, nothing is hidden. Every effect has a
  `prefers-reduced-motion` path (Lenis off → native scroll; entrances skipped).

### The Telemetry Rule (monospace)

Monospace (`Spline Sans Mono`) is **not** decorative "tech" costume — it is the trip's
data voice. It carries only the *logbook layer*: clock times, mileage, coordinates, prices,
charge-stall counts, countdown digits (tabular, so they don't jitter), and romanized
English subtitles beneath their 中文 names. Prose, headlines, and display stay
Playfair / Work Sans. If a string isn't a number, a time, a measurement, or a romanization,
it does not get mono.
