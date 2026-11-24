---
name: Mission Objective
description: Tentative design system for Mission Objective, a women-run product design and innovation studio. Dark, minimal, Inter-only. Currently focused on three-slide LinkedIn case-study carousels.
status: tentative (brand in progress)
colors:
  background: "#111418"
  surface: "#16191b"
  surface-raised: "#1d222a"
  on-background: "#f5f0f3"
  on-background-muted: "#a5afc0"
  line: "#2d3643"
  line-strong: "#617189"
  signal: "#dcf471"
  on-signal: "#111418"
  signal-text: "#dcf471"
  pop: "#95eeec"
  on-pop: "#111418"
  highlight: "#314fab"
  on-highlight: "#dcf471"
  client-default: "#314fab"
  focus: "#2a74f5"
  light-background: "#f5f0f3"
  light-on-background: "#111418"
  light-on-background-muted: "#455368"
  light-signal-text: "#424e13"
  light-highlight: "#dcf471"
typography:
  display-xl: {fontFamily: Inter, fontSize: 112px, fontWeight: 200, lineHeight: 108px, letterSpacing: -0.035em}
  display: {fontFamily: Inter, fontSize: 72px, fontWeight: 300, lineHeight: 72px, letterSpacing: -0.03em}
  headline: {fontFamily: Inter, fontSize: 44px, fontWeight: 300, lineHeight: 48px, letterSpacing: -0.02em}
  title: {fontFamily: Inter, fontSize: 24px, fontWeight: 400, lineHeight: 32px, letterSpacing: -0.01em}
  body-lg: {fontFamily: Inter, fontSize: 20px, fontWeight: 300, lineHeight: 30px}
  body: {fontFamily: Inter, fontSize: 16px, fontWeight: 300, lineHeight: 1.5}
  caption: {fontFamily: Inter, fontSize: 13px, fontWeight: 400, lineHeight: 18px, letterSpacing: 0.01em}
  label: {fontFamily: Inter, fontSize: 18px, fontWeight: 300, lineHeight: 24px, letterSpacing: 0.01em, textTransform: uppercase}
  eyebrow: {fontFamily: Inter, fontSize: 12px, fontWeight: 500, lineHeight: 16px, letterSpacing: 0.12em}
rounded:
  none: 0
  sm: 4px
  md: 12px
  lg: 24px
  pill: 999px
  round: 50%
  letter: 19.6%
  letter-outer: 37.3%
spacing:
  xs: 4px
  sm: 8px
  ms: 12px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 48px
  3xl: 64px
  4xl: 96px
  5xl: 128px
components:
  case-study-slide:
    width: 540px
    height: 675px
    backgroundColor: "{colors.client-default}"
    textColor: "{colors.on-background}"
    rounded: "{rounded.letter}"
    padding: "{spacing.2xl}"
  highlight:
    backgroundColor: "{colors.highlight}"
    textColor: "{colors.on-highlight}"
    rounded: "{rounded.none}"
---

# Mission Objective design system

## Overview

Mission Objective is a women-run product design and innovation studio. The brand is still being decided, so every value here is tentative and meant to be iterated; change a token, then re-check the contrast pairs and the "why" of any template that uses it.

**Brand personality.** Chic (simple, not plain), minimalist and understated, smart, a little cheeky, sophisticated but slightly irreverent, independent, optimistic, futuristic, warm and thoughtful, direct and honest. More NASA than military: wordplay on "mission" and "objective" is fine; war language is not.

**Voice.** Sentence-case headlines, full stops allowed, "we" for the studio and "you" for the client, no emoji, short paragraphs. Example: "Mission Objective is a product design and innovation studio."

**Direction after team critique.** The team leans toward a minimal, sophisticated look. The earlier "communique" route (type and color only) was closest but felt close to too safe or bland. Templates must be restrained but not bland: visual interest comes from intentional design and attention to detail, not from flash or editorial effects. Every design decision needs a tangible "why" that points back to the brand (a measurement from the logo, a brand value, a hierarchy rule); "it looks nice" is not a reason. Templates are lightly branded so they never compete with client branding in a case study. Dark backgrounds are preferred because they stand out on LinkedIn's white feed.

## Colors

The palette is five ramps with ten steps each (050 lightest to 900 darkest), taken from the team's Figma color table. Name raw colors as `ramp-step`, for example `lime-200`.

| step | grey | stone | lime | cyan | blue |
|---|---|---|---|---|---|
| 050 | `#f0f1f5` | `#faf8f8` | `#f8fde3` | `#e0fafa` | `#f3f4fc` |
| 100 | `#d8dce4` | `#ece8e8` | `#ebf9ae` | `#bdf4f4` | `#e2e8f8` |
| 200 | `#c0c7d3` | `#d8cecf` | `#dcf471` | `#95eeec` | `#c9d3f3` |
| 300 | `#a5afc0` | `#beb0b1` | `#c9e453` | `#44dfdb` | `#a8b9eb` |
| 400 | `#8895aa` | `#9b8889` | `#b3cf3f` | `#33c1be` | `#7f98e1` |
| 500 | `#617189` | `#746264` | `#95ae32` | `#29a3a1` | `#4a6dd4` |
| 600 | `#455368` | `#564749` | `#687a1f` | `#257e7d` | `#314fab` |
| 700 | `#2d3643` | `#3b3031` | `#424e13` | `#144847` | `#22346d` |
| 800 | `#1d222a` | `#241d1e` | `#242c07` | `#0e2a29` | `#162140` |
| 900 | `#13161b` | `#191616` | `#161c01` | `#071818` | `#0e1425` |

Legacy names still in the system: `White` #ffffff, `Black` #111418 (the dark ground), `Grey` (= grey-200), `Iron`, `Lime` (= lime-200), `Cyan` (= cyan-200), `paper` #f5f0f3 (light ground and light text), and the aurora set `aurora-green` #dcf471, `aurora-teal` #144847, `aurora-blue` #4a6dd4, `aurora-violet` #5b4fc0 (website glow only).

**Semantic roles (dark theme, default).** `background` #111418; `surface` #16191b; `surface-raised` #1d222a; text `on-background` #f5f0f3; secondary text `on-background-muted` #a5afc0; `signal` #dcf471 (lime fill; text on it `on-signal` #111418); `signal-text` #dcf471 for emphasized words and thin marks; `pop` #95eeec (second highlight, fill only); `highlight` #314fab with `on-highlight` #dcf471 (a text-selection look); hairlines `line` #2d3643 (decorative) and `line-strong` #617189 (carries meaning).

**Light theme.** `background` #f5f0f3, text #111418, secondary text #455368, `signal-text` #424e13, `highlight` is a lime marker #dcf471 with #111418 text.

**Pairing rule.** Grounds at steps 200-300 take Black or step 700-800 ink; grounds at 600-900 take step 100-200 ink, or Lime/Cyan for the wordmark and highlights. Use one highlight color per layout.

**Contrast (checked).** paper on Black 16:1; grey-300 on Black 8:1; lime-200 on Black 15:1; Black on lime-200 15:1; lime-200 on blue-600 6:1; paper on blue-600 6.6:1; line-strong on Black 3.7:1. Muted text (`grey-300`) is not used on a client-color ground (3.4:1 on blue-600); use `on-background` there.

## Typography

Inter only, light weights. Display and statements at 200-300 with tight tracking, running text at 300, labels uppercase. Scale as in the front matter. At the 540 px slide canvas the token sizes apply 1:1: `headline` for cover statements and pull-quotes, `body` for supporting lines, `body-lg` for artwork captions, `caption` for attributions, `eyebrow` for the client name and slide count.

## Layout

**Case-study canvas.** 4:5 portrait, 540 x 675 at 1x, exported at 2x as 1080 x 1350 (a portrait slide takes more of the mobile feed). Outer margin `2xl` (48px). Spacing names here map to the design system's `space-1` to `space-10` (xs=space-1 ... 5xl=space-10; sm=space-2 8px, md=space-4 16px, lg=space-5 24px, 2xl=space-7 48px). Spacing otherwise uses the scale above; keep left-aligned type and generous empty space. Hairlines (1px) are the main structural device.

## Elevation & Depth

Flat. No shadows or gradients in templates. (`shadow-lift` exists for rare floating UI.) Depth comes from layering one panel over a color ground.

## Shapes

All curves come from the logo, so they can be explained.

Measured from the white wordmark SVG, the "O" of OBJECTIVE is a rounded rectangle 41.0 wide by 45.8 tall (units) with:

- outer corner radius about 17.1 units = **37.3%** of cap height (`rounded.letter-outer`),
- counter (inner hole) corner radius about 9.0 units = **19.6%** of cap height (`rounded.letter`),
- stroke thickness about 8.8 units = 19.3% of cap height.

Use `rounded.letter` on a square element so the percentage stays circular (the slide panel is a square the height of the slide). Everything else in templates is square (`rounded.none`), including highlighted-word fills, because text selections are square.

## Components

### Case-study slide (three per case study)

A client-color ground with a dark panel inset from its left edge. Read it as the O: the client color is the letter and the dark panel is its counter. The panel's bottom-left corner uses `rounded.letter`; a 24px sliver (`spacing.lg`) of client color shows to its left. The header holds the client name (left), a `NN / 03` count (right) and a 1px progress rule whose lime segment fills 1/3, 2/3, 3/3. The Mission Objective wordmark is bottom right, 28px high.

| Slide | Content | Type |
|---|---|---|
| 01 Cover | A statement of what we did and the value we offered; one support line | `headline`, `body` |
| 02 Artwork | A mockup or image of the work, flush with the content margins, plus a one-line caption | `body-lg` |
| 03 Quote | Client pull-quote with lime quote mark and attribution (name, role, client). Option: full client-color ground | `headline`, `caption` |

**Why each decision stands**

| Decision | Reason it points back to the brand |
|---|---|
| Dark ground (`background`) | Stands out on LinkedIn's white feed; matches the website ground; reads as sophisticated and futuristic. |
| Client name and color lead, our wordmark is small and bottom right | The case study is the client's story; our branding must not compete with theirs. Direct and honest. |
| Panel curve = `rounded.letter` from the O's counter; client color is the letter | Geometry is measured from our own logo, so the frame is a magnified piece of the mark: understated, but explainable. |
| 24px sliver of client color (`spacing.lg`) | Smallest spacing step that still reads as color rather than a border; keeps the client color present but quiet. |
| Progress rule with a lime segment | It is the pagination and the brand's only ornament: the three-slide structure becomes visible without extra decoration. Direct. |
| Emphasis on 1-3 words in lime, or a selection-style `highlight` fill | Marking the objective echoes "mission objective" and highlighting text on screen; adds interest and color to a minimal layout. Square corners, like a selection. |
| Inter 300, sentence case, tokens only | Matches the website's light hero type; one family, one weight range, no editorial flourishes. |
| One accent (lime), blue only as client/selection | A second accent would compete with client branding and break the restraint. |

### Highlight (inline)

Wrap the words in `**double asterisks**` in slide copy. Mode `text`: color `signal-text`. Mode `highlight`: `highlight` fill, `on-highlight` text, `rounded.none`. On a client-color ground the fill is `background` with lime text so it does not vanish into blue. Use one mode per series and one emphasis per slide.

### Other pieces

Button (solid, accent, outline; 8px / 24px padding, `rounded.md`), Tag (uppercase pill, 8px / 16px padding), ServiceList (right-aligned uppercase rules, from the website), Aurora (website glow background, not for templates), SocialPost (earlier 1:1 explorations, kept for reference).

## Do's and Don'ts

- Do keep slides dark, flat, left-aligned and mostly empty; let the client's artwork carry the visual weight.
- Do write the brand reason for any new template decision next to it.
- Do keep emphasis to one to three words per slide and one highlight mode per series.
- Don't add gradients, shadows, textures, second logos, extra accent colors or decorative shapes.
- Don't put muted grey text on a client-color ground.
- Don't redraw, recolor or restyle the logo; use the supplied SVGs (white on dark, black on light).
- Don't use the aurora glow, crosshairs, or tile grids in case studies (explored, parked as too loud or too decorative).

## Open questions

Final highlight color; curves from the E and M of the wordmark (the Figma explores them); event banner format (16:9, 1280 x 720); photography direction; light-theme templates.
