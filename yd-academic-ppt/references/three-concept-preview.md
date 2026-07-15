# Three-concept full-deck preview

This stage is mandatory for academic, editable pitch, creative pitch, and poster routes unless the user explicitly waives it. It produces visual-selection boards before PPTX authoring.

## 1. Output contract

Deliver in this order, with an outline-confirmation boundary between steps 1 and 2 unless the user explicitly authorizes automatic continuation:

1. a concise outline/slide map;
2. concept A contact sheet;
3. concept B contact sheet;
4. concept C contact sheet;
5. a short comparison of the three visual systems;
6. one selection request: A, B, C, or a precisely defined hybrid.

A contact sheet is one high-resolution PNG/JPEG containing every 16:9 slide thumbnail in order. It is not a PDF and not a substitute for the final PPTX/PDF.

## 2. Story lock

Create one structured source of truth before visual divergence. For every slide lock:

- slide ID and order;
- exact takeaway title;
- one-sentence purpose;
- required facts, numbers, equations, citations, and terminology;
- content blocks and their priority;
- evidence/asset source;
- estimated speaking time;
- logo, author, institution, section, and pagination requirements.

Show the slide map and obtain confirmation before generating all concept pages. Concepts A/B/C must then use the same slide count, order, governing thesis, claims, data, citations, logo policy, and conclusion. They may vary composition, typography, palette, visual metaphor, chrome, card/table morphology, texture, and density rhythm. Do not let ImageGen rewrite the narrative.

## 3. Build three genuinely different systems

Each concept needs a one-page style bible covering:

- 4–8 descriptive art-direction keywords;
- palette with dominant, structural, accent, background, and text colors;
- title/body typography personality;
- header/footer/page-number language;
- grid and whitespace rhythm;
- cards, tables, charts, icons, diagrams, and image framing;
- recurring motif and visual continuity device;
- image rendering style, lighting, texture, and depth;
- density target and negative constraints.

The concepts must be meaningfully different, not one design with three color swaps. For default academic topics, concept A should be the high-fidelity YD navy/red editorial system from `academic-template-fidelity.md`; B and C should remain credible and formal while varying modern research expression and technical/analytical character. If the user supplies another template, replace A with that source-led direction. For creative projects, derive all three from the project world rather than choosing unrelated fashionable styles.

## 4. Generation sequence

Internally validate three keyframes per concept before expanding the entire deck: cover, densest content page, and chart/table/process page. Once the style is coherent, generate every page in that concept.

Use a shared master prompt plus a slide-specific prompt. Every prompt should define:

1. complete 16:9 presentation slide, not a mockup;
2. slide role and story-lock ID;
3. exact title and required short labels;
4. content hierarchy and reading order;
5. composition zones and safe margins;
6. selected style bible verbatim;
7. recurring header/footer/motif rules;
8. visual anchor and supporting elements;
9. table/chart/process visual relationship when applicable;
10. density and whitespace target;
11. continuity with the same concept's prior pages;
12. negative constraints: no random copy, fake data, fake logo, template drift, cropped title, illegible microtext, or unrelated decoration.

Use the cover/keyframes as visual references for later pages when the generation system supports image conditioning. Reuse palette, border language, illustration treatment, icon family, lighting, and typography personality across the concept.

## 5. Academic preview rules

- ImageGen may design the entire page, including background, frame, panels, diagrams, imagery, and typographic hierarchy.
- Prefer short display copy and clear structured containers. Do not ask the model to invent dense factual paragraphs or numerical tables.
- Use the story lock as the textual source of truth. If generated text is malformed, regenerate or place exact text over the generated composition before rasterizing the preview slide.
- Exact charts, tables, equations, citations, and research results must come from source data or supplied material. Preview decoration must never masquerade as evidence.
- Design for later separation: distinct content zones, clean boundaries, predictable z-order, and enough contrast to reconstruct native objects.

## 6. Creative/hackathon preview rules

- Generate each page as a complete high-impact image with integrated artistic lettering and project-specific world-building.
- Exact names, numbers, slogans, and required labels remain locked and must be checked at full resolution.
- Richness is allowed, but one focal point, one dominant headline, and a consistent campaign identity are mandatory.

## 7. Contact-sheet construction

Generate individual slide images first; never ask ImageGen to hallucinate the whole deck as one miniature collage. Compose the board deterministically afterward.

- 8 slides: normally 4 × 2.
- 12 slides: normally 4 × 3.
- 20 slides: normally 5 × 4.
- Other counts: choose the fewest rows that preserve readable thumbnails.
- Keep every thumbnail uncropped at 16:9 with equal gaps.
- Add concept name and slide numbers outside the slide frames.
- Use a neutral board background that does not contaminate the concept palette.
- Output at sufficient resolution for zoom review; target at least 320–480 px width per thumbnail.
- Check for missing, duplicated, reordered, or differently sized pages.

## 8. Selection boundary

Do not create the final PPTX/PDF before the user selects a concept. A hybrid is allowed only when specified as attributes, for example: “A's frame and typography + C's chart language.” Resolve conflicts into one style bible before continuing.
