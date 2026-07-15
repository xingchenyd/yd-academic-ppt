# Image-to-editable academic reconstruction

Use only after the user selects an academic concept. The approved full-slide images are the visual source of truth; the story lock and source ledger are the semantic source of truth.

## 1. Reconstruction objective

Rebuild each page so the rendered PPTX is extremely close to the approved image in silhouette, geometry, color, hierarchy, typography, border language, spacing, and visual weight while preserving exact text/data and practical editability. Do not promise literal pixel identity unless measured; target near-pixel visual similarity for stable layout regions.

## 2. Create a per-slide scene graph

Before authoring, inventory every visible element with:

- element ID and semantic role;
- normalized bounding box `(x, y, w, h)` and alignment anchors;
- z-order, grouping, clipping, rotation, corner radius, stroke, fill, opacity, and shadow;
- reconstruction class;
- content source and exact text/data;
- required editability;
- confidence and fidelity risk.

Use five reconstruction classes:

1. **Native text:** titles, body, labels, captions, citations, page numbers, badges.
2. **Native geometry:** backgrounds, panels, borders, lines, arrows, simple icons, dividers, basic diagrams.
3. **Native data object:** tables, charts, equations, timelines, matrices, and data-driven diagrams.
4. **Separate visual asset:** photos, illustrations, official logos, screenshots, complex icons, scientific figures, textures, and 3D art placed as individually movable/croppable image or SVG objects.
5. **Complex visual plate:** non-informational atmosphere, lighting, scenery, material texture, or an inseparable decorative region retained as a background/region image.

## 3. Clean-plate and asset extraction

Never place the approved page as a final full-slide background and cover its text with editable text; this creates ghosting and false editability.

Instead:

1. create a clean plate by editing/inpainting the selected image to remove text, tables, charts, simple panels, and any element that will be rebuilt;
2. preserve only complex background atmosphere and deliberately inseparable decoration;
3. isolate important photos/illustrations/logos/screenshots into separate assets when feasible;
4. remove each isolated asset from the clean plate before placing it back as a separate object;
5. use masks sampled from nearby background colors only for small repairs; avoid visible patches, repeated texture, or halos;
6. keep the approved page available as a temporary alignment reference, then remove it from the final export.

If extraction would visibly damage a complex visual, retain that bounded region as one image and rebuild its major text outside the raster. State any material editability exception.

## 4. Text reconstruction

- Take exact wording from the story lock/source, not OCR. OCR may help locate text but never overrides the approved copy.
- Match font category and visual character first, then size, weight, color, line spacing, tracking, alignment, and line breaks.
- Prefer the closest installed font; if unavailable, choose the nearest visual substitute and recalibrate size/spacing.
- Preserve colored keywords, bold spans, numbering, quotation marks, units, subscripts/superscripts, and citation styling.
- Reject missing glyphs, wrong line breaks, overflow, text drift, or baseline mismatch.
- If exact source layout harms legibility after native rendering, allow only a small semantic-preserving adjustment and record it.

## 5. Tables, charts, formulas, and diagrams

- Rebuild tables natively with exact rows, columns, values, merges, fills, borders, padding, and emphasis.
- Rebuild charts from source data whenever available. Do not infer values from pixels.
- If only an image chart exists, either retain it as an editable image object or reconstruct a visually approximate chart and label the internal QA ledger `data unavailable—visual approximation`; never invent precision.
- Rebuild formulas with editable math/text and verify symbols manually.
- Rebuild simple flows and geometry natively; preserve complex scientific or artistic diagrams as bounded image assets when redrawing would reduce fidelity.
- Official logos, UI screenshots, people, products, and branded imagery must come from supplied/original assets, not hand-drawn imitation.

## 6. Calibration and batch reconstruction

Select a dense representative page containing at least two of: table, chart, diagram, complex image, multiple cards, or a takeaway strip.

1. reconstruct it fully;
2. render at the same aspect ratio/resolution as the approved image;
3. compare side by side and with a 50% opacity registration overlay;
4. correct global tokens and reusable helpers;
5. freeze the system only after the page passes;
6. reconstruct the remaining pages using the same helpers but page-specific scene graphs.

## 7. Fidelity scoring

Score each reconstructed page out of 100:

- silhouette, composition, and reading order: 25;
- position, size, alignment, and spacing: 20;
- typography and text hierarchy: 20;
- palette, contrast, borders, radii, and effects: 15;
- table/chart/component morphology: 10;
- complex assets, texture, and detail: 10.

Target at least 90/100 for every page and 94/100 for cover, overview, densest evidence page, and closing. Accuracy and readability remain hard gates even when a visual score passes.

## 8. Final editability audit

Confirm that:

- all ordinary text is selectable and editable;
- tables and data-bound charts are editable where source data exist;
- simple shapes, lines, arrows, and page furniture are native objects;
- each retained image is independently selectable, movable, crop-adjustable, and replaceable where feasible;
- no invisible reference slide image, duplicate text, masking seam, or rasterized factual table remains;
- PPTX and PDF renders match without clipping or font substitution.

Editability means practical object-level editing, not that photographs, paintings, textures, or complex scientific figures become fully vectorized.
