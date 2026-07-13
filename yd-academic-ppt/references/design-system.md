# YD editorial design system

## 1. Design character

Formal, scholarly, calm, precise, information-rich, and visibly structured. The visual language should feel like a premium academic briefing or carefully edited teaching handout—not a corporate dashboard, social-media carousel, or decorative keynote.

## 2. Canvas, frame, and grid

- Default to 16:9 widescreen.
- Use a 12-column mental grid with equal left/right safe margins.
- In the default academic route, reserve a real top identity zone and bottom navigation band; do not reduce them to hairlines. The top-left navy tab should occupy roughly 36–43% of slide width and 7–10% of slide height. The bottom band should occupy roughly 5–7% of slide height.
- Align all major edges to a small set of x-coordinates.
- Use 8–16 px-equivalent internal spacing increments consistently.
- Prefer 2–4 principal regions per slide; use 5–7 only for intentionally repeated small categories.

## 3. Palette

Default palette; adjust slightly for institution branding while preserving contrast:

| Role | Color |
| --- | --- |
| Warm canvas | `#F7F3EC` |
| Primary navy | `#082B4F` |
| Secondary navy | `#123F68` |
| Decision red | `#A5161A` |
| Deep red | `#7E1014` |
| Muted gold | `#B99A4A` |
| Main text | `#14273B` |
| Secondary text | `#465361` |
| Hairline border | `#D5D0C8` |
| Soft panel | `#FBF9F5` |

Use navy for structure and continuity; red for contrast, risk, decisions, highlights, or alternating steps. Use gold sparingly for seals or premium institutional accents. Never use pale gray for essential text.

## 4. Typography

Prefer editable, widely available fonts and design typography deliberately. Never use plain black Song text as an unstyled default. For the default academic route, use a strong high-contrast Chinese serif for the main title—prefer Source Han Serif/Noto Serif CJK SC SemiBold/Bold—and a clean Chinese sans/Hei face for body copy—prefer Source Han Sans/Noto Sans CJK SC. Use a heavy sans title only when the user requests a modern technical variation. For pitch routes, choose a theme-appropriate display font plus a highly readable body font. For mixed Latin/math, use a compatible serif for equations and a clean sans serif for labels.

Recommended starting sizes for 16:9:

| Element | Size |
| --- | --- |
| Cover title | 36–48 pt |
| Content title | 29–36 pt, default serif, visually dominant |
| Subtitle/deck thesis | 18–24 pt |
| Card header | 17–22 pt |
| Body | 16–20 pt; prefer 18+ for projection |
| Table/chart label | 14–18 pt, never below 12 pt |
| Footer/page marker | 10–13 pt |

Shorten or split before shrinking. Keep title weight visibly stronger than body. Use red only for selected key phrases, not entire paragraphs.

Use two font families at most, plus a monospace face only when code or technical labels require it. Use weight, color, size, tracking, case, and line spacing to create hierarchy; do not rely on font family alone.

## 5. Signature chrome — mandatory in template-fidelity mode

- Top-left: substantial navy polygon/banner, flush to the top and left edges, with a clipped or angled right end. Add an optional gold-outlined emblem plus white series/institution text. It must read as a color block, not a 2–4 px rule.
- Top-right: 3–4 short values or deck traits in navy, separated by thin vertical bars, aligned inside the same top identity zone.
- Section eyebrow: red section name plus navy descriptor.
- Title: dark navy numbered badge, large navy serif headline, and a short red underline 0.45–1.1 in wide and roughly 3–5 pt thick, aligned to the left title edge. The badge should sit on the title baseline, not float as a separate dashboard tile.
- Footer: full-width navy band, flush to the bottom edge, with identity/tagline on the left; overlay a red angled tab on the right for section, subsection, and pagination. Keep page notation such as `03/05` inside the tab.

Replace all source branding with the user's title, lab, institution, course, or a neutral series name. Omit this chrome only for an explicit institutional template, frameless conference style, or user request.

## 6. Components

- Cards: warm white fill, 0.75–1 pt neutral/navy-tinted border, visibly rounded 0.08–0.14 in corners, minimal/no shadow. Square corners are a defect in template-fidelity mode.
- Card headers: navy or red bands with rounded top corners and white text; alternate only when the distinction is meaningful. For unfilled cards, use a circular navy/red icon plus a colored header label.
- Icons: one coherent line/solid family, high contrast, contained in circles or simple badges. Do not mix emoji with professional icons.
- Takeaway strip: bottom-row summary with 3–5 compressed claims; use only when it adds memory value.
- Tables: embed the native table in a rounded outer card; use a dark navy title/header band, white bold labels, compact rows, restrained warm zebra shading, light horizontal separators, and one red-highlighted result row/cell at most. Avoid spreadsheet-like full grids and oversized rows.
- Charts: navy/red primary series, gray context series, direct labels when practical, minimal gridlines.
- Equations: generous whitespace, clear variable legend, and a nearby interpretation in plain language.

## 7. Visual restraint

Avoid gradients, glossy effects, 3D charts, excessive rounded pills, floating UI widgets, thick shadows, clip-art collage, decorative photos, and random color coding. Use illustrations only when the subject materially benefits. Prefer domain figures, data, diagrams, and evidence.
