# Poster-led impact / full-image mode

## Mode contract

This is the full-image final-output route for hackathon pitches, creative product launches, game concepts, campaign decks, and promotional presentations. Normal creative decks may use controlled density; the intentionally extreme poster treatment is a stronger sub-mode for users who prioritize maximum visual impact over restraint.

Generate every final slide as one complete 16:9 AI-rendered page image. The bitmap contains everything visible:

- background and environment;
- characters, products, devices, scenes, props, and hero objects;
- artistic Chinese/English title lettering;
- subtitles, labels, stickers, badges, callouts, short explanatory copy, and page markers;
- diagrams, stylized flows, UI-like frames, decorative patterns, textures, lighting, particles, and brand chrome.

Do not reconstruct the approved page with PowerPoint objects. Assemble each approved full-slide image edge-to-edge into `.pptx` and export the matching PDF. State clearly at delivery that element-level editing is unavailable in this mode.

## Trigger boundary

Use image-based assembly by default for hackathon and creative pitch routes. Escalate to the **extreme poster** treatment only when the user explicitly requests one or more of:

- poster-like or promotional full-slide visuals;
- very strong visual impact or infectious stage presence;
- full-page ImageGen output;
- abundant artistic lettering and integrated visual text;
- a style comparable to a high-energy hackathon show deck, game poster, campaign launch, or visual concept deck;
- non-editable output and maximum visual density are acceptable.

A normal startup/business presentation that is formal, investor-document-like, or explicitly editable may instead use editable reconstruction. Do not assume every business deck needs extreme poster density.

## Production chain

Create and preserve a private production package:

1. **Brief:** audience, venue, duration/page count, project promise, emotional target, mandatory facts, exact names, logos, and source assets.
2. **Storyline:** hook → tension/opportunity → concept → core experience → mechanism/demo → differentiation → proof → impact → roadmap/ask → closing.
3. **Copy lock:** approve or infer the exact short text for every page before generation. Reduce prose into poster-scale phrases, but preserve required terminology and numbers.
4. **Design system:** visual world, palette, type personality, composition rhythm, image style, recurring motifs, logo/header/footer treatment, density, and negative constraints.
5. **Storyboard/story lock:** page role, exact title/copy, focal object, supporting labels, evidence, continuity cue, and QA risks. This content remains identical across concepts.
6. **Three visual systems:** create A/B/C style bibles and follow `three-concept-preview.md` to generate three complete decks and contact sheets.
7. **Selection:** pause for the user's choice or explicit hybrid; do not assemble a final PPTX before selection.
8. **Full-resolution repair:** inspect every selected image. Use image editing or regenerate the complete slide when any visual/textual defect appears.
9. **Assembly:** place each approved image edge-to-edge on a 16:9 slide without overlays, margins, cropping, or letterboxing; export PPTX and PDF.

## Long-prompt structure

Every slide prompt should normally specify all relevant fields:

1. **Deliverable:** complete 16:9 presentation slide/poster, exact resolution, no mockup border.
2. **Slide role:** cover, problem, concept, core loop, product demo, technology, business value, roadmap, closing, etc.
3. **Exact visible text:** list every required phrase verbatim, with language, capitalization, punctuation, and hierarchy.
4. **Visual world:** project-specific setting and emotional atmosphere.
5. **Hero focal point:** one dominant character, device, product, portal, map, installation, scene, or symbolic object.
6. **Composition:** left/right/center hierarchy, reading direction, safe margins, visual balance, and where each text group belongs.
7. **Typography:** artistic lettering personality, stroke, outline, shadow, perspective, texture, color, and scale relationships.
8. **Secondary elements:** supporting characters, cards, stickers, arrows, badges, icons, diagrams, screens, charts-as-decoration, and environmental details.
9. **Palette and lighting:** exact dominant/accent colors, contrast, glow, texture, depth, and rendering finish.
10. **Recurring identity:** logos supplied by the user, project mark, page number system, header/footer motif, and repeated symbols.
11. **Density:** intentionally rich and layered, with many coordinated elements, but a clear focal point and readable visual hierarchy.
12. **Negative constraints:** no random text, no fake logos, no misspellings, no cropped headline, no bland office template, no unrelated stock elements, no illegible microtext, no chaotic overlap.

Prompts should be long enough to control the full composition. Do not rely on vague requests such as “make it cool” or “cyberpunk PPT.”

## Density and art direction

Full-image mode may use many elements and much more decorative density than the other routes. Richness must still be organized:

- Establish one dominant focal object and one dominant headline.
- Use multiple secondary elements to build a world, explain a loop, or create stage energy.
- Repeat a controlled motif family rather than unrelated decoration.
- Vary slide compositions while preserving the same palette, typography personality, rendering style, border language, and brand chrome.
- Treat every page as a designed poster and the whole deck as one visual campaign.
- Make the cover, core experience, demo, proof, and closing pages especially memorable; do not allow weak middle pages.

## Text-generation rules

Extensive generated text is allowed in this mode, including artistic Chinese titles and English display words. Accuracy is still mandatory.

- Lock exact wording before generation.
- Prefer short lines, strong verbs, memorable phrases, and limited paragraph length.
- Inspect every Chinese character, English word, number, punctuation mark, and product name at full resolution.
- Reject warped glyphs, pseudo-Chinese, fake English, random filler, inconsistent product naming, and unreadable small copy.
- If text is wrong, revise the prompt and regenerate or edit the full image. Do not cover it with a local PowerPoint text box.
- If a page repeatedly fails because it contains too much exact copy, shorten or split the page while preserving the narrative.

## Full-slide QA gates

- Every expected slide exists and matches the storyboard order.
- Every final image is landscape 16:9 with consistent resolution.
- The full-slide image reaches all four edges without padding or letterboxing.
- Exact titles, labels, names, numbers, and slogans are correct.
- No random symbols, fake logos, malformed hands/faces/products, broken UI, or distorted charts appear.
- Important content stays inside safe margins.
- Each page has a clear focal point despite high element density.
- Palette, rendering style, typography personality, chrome, and motif language remain consistent.
- The cover and closing feel intentionally designed and stage-ready.
- The PPTX contains one full-page image per slide and the PDF visually matches it.
