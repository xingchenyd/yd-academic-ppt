# Visual generation and editable-text policy

## Two-stage contract

At concept stage, ImageGen is the principal full-page art director for all routes. At final stage, output rules diverge:

- academic: selected images become reconstruction targets; factual information is rebuilt natively;
- hackathon/creative/poster: selected images remain the final full-slide visuals and are assembled directly;
- editable creative pitch: reconstruct only when explicitly requested.

In final academic output, native editable information includes:

- titles and subtitles;
- paragraphs and bullets;
- labels, legends, captions, callouts, citations, and page numbers;
- tables, chart labels, formulas, timelines, and process steps;
- product feature names, metrics, and evidence statements.

Do not default to black Song typography. Select a type system for the route and use purposeful color, weight, size, alignment, tracking, and emphasis. Verify that chosen fonts are installed or use safe fallbacks.

## Full-page academic concept exception

Before selection, generate each academic slide as a complete 16:9 visual composition. ImageGen may create the frame, background, panels, visual hierarchy, illustrations, decorative geometry, and proposed typography. Use exact native/raster overlays on the preview image when necessary to prevent malformed factual text. The preview is a design target, not the final evidence artifact.

After selection, follow `image-to-editable-reconstruction.md`. Do not leave AI-rendered paragraphs, numerical tables, equations, citations, or charts as raster content in the final academic deck when native reconstruction is feasible.

## Accuracy prohibitions

Never allow ImageGen to invent:

- fake logos, fake screenshots, fake app interfaces, fake papers, or fabricated evidence;
- a collage of many unrelated AI assets merely to fill empty space.

AI-generated charts/tables may appear only as non-evidentiary composition placeholders in concept boards. Replace them with exact source-bound native objects in final academic output.

## Artistic display lettering

Academic concepts may explore stylized display lettering, but final academic titles should normally be reconstructed as editable type. Keep generated lettering as an image only when the user explicitly accepts that local editability exception and every glyph is correct.

- Limit generated lettering to one short title, slogan, or logo-like wordmark per selected slide.
- Verify every character against the approved wording at full resolution.
- Regenerate if any glyph, spacing, punctuation, or English spelling is wrong.
- Keep all explanatory and factual text native and editable.
- Record the exact wording in speaker notes or the private storyboard as the source of truth.
- Do not use generated lettering on every slide; reserve it for cover, section impact, or a decisive closing page.

## Creative full-image final output

For hackathon/creative/poster output, the selected concept is intentionally retained:

- Generate the complete slide as one unified 16:9 bitmap.
- Permit extensive artistic titles, integrated labels, badges, visualized steps, stylized UI-like panels, and decorative microcopy inside the generated image.
- Do not add native PowerPoint text, shapes, charts, or local repair layers on top of the final approved slide.
- Expect the resulting PPTX to be image-based and non-editable at element level.
- Use [poster-impact-mode.md](poster-impact-mode.md) as the controlling reference.

## Restraint and consistency

- Use one dominant visual metaphor or hero object per slide.
- Prefer a repeated asset family across a section over newly generated unrelated art on each page.
- Keep decorative assets subordinate to the message.
- Match perspective, lighting, rendering style, outline language, texture, and palette across the deck.
- Never let generated art reduce readability or evidence credibility.
