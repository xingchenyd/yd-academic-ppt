# QA rubric

Score each category 0–2. Do not deliver below 18/20, and do not allow a zero in accuracy, readability, or technical integrity.

| Category | 0 | 1 | 2 |
| --- | --- | --- | --- |
| Purpose | Unclear | Partly clear | Governing message and audience outcome are explicit |
| Narrative | Disconnected | Mostly logical | Titles alone reveal a coherent argument |
| Accuracy | Unsupported/errors | Minor gaps | Claims, numbers, formulas, and citations verified |
| Content selection | Important gaps/no prioritization | Mostly complete | Complete, prioritized, and time-appropriate |
| Readability | Tiny/low contrast | Some dense areas | Legible at intended viewing distance |
| Hierarchy | Flat/confusing | Mostly consistent | Title, evidence, annotation, takeaway are instantly distinct |
| Layout | Overflow/misalignment | Small inconsistencies | Clean grid, spacing, balance, and varied silhouettes |
| Visual evidence | Decorative/misleading | Adequate | Charts/figures directly support claims and are interpretable |
| Consistency | Mixed styles | Minor drift | Tokens, cards, icons, charts, header/footer are coherent |
| Technical integrity | Broken output | Minor conversion differences | Route-correct PPTX/editability, faithful PDF, no clipping/overlap/placeholders |

## Required visual inspection

1. Render every PPTX slide to PNG.
2. Inspect every slide individually at full size.
3. Inspect a montage for pacing, repetition, and color balance.
4. Run overflow/slide-bound tests.
5. Export PDF and render representative PDF pages, including the densest slide, a chart/table slide, and the final slide.
6. Compare PPTX and PDF for fonts, line breaks, equations, charts, and page edges.
7. For the academic route, compare the montage and at least three full-size slides against `academic-template-fidelity.md`. Color match alone does not pass.

## Three-concept preview gate

Before requesting selection, verify all of the following:

1. A/B/C contain the same number of slides in the same order.
2. Titles, claims, evidence, numbers, conclusion, and logo policy match the story lock.
3. Each concept is internally consistent from cover to closing.
4. The three concepts differ materially in more than palette.
5. Every slide is visible, uncropped, correctly numbered, and readable enough for visual selection.
6. No contact sheet contains duplicate/missing pages, random copy, fake evidence, or style drift.
7. No PPTX/PDF is delivered before selection unless the user explicitly waives the concept stage.

## YD academic template-fidelity gate

Apply this gate when the selected concept is the default YD academic system or the user requests fidelity to the original reference. For another selected academic style, apply the same structural rigor using its style bible rather than forcing navy/red chrome. All seven checks must pass when this gate applies:

1. A substantial navy top-left banner and a full-width navy/red footer are present on applicable slides.
2. The title uses the serif-number-badge-red-underline lockup at reference-like scale.
3. Repeated cards have visibly rounded corners and consistent padding; no accidental square dashboard boxes remain.
4. Tables use compact editorial construction rather than a plain spreadsheet grid.
5. The central layout has reference-like density and semantic iconography without crowding.
6. The header, title block, content grid, takeaway strip, and footer align to a common geometry.
7. Source branding/watermarks are replaced, while the structural identity is preserved.

## Image-to-editable fidelity gate

For the selected academic concept:

1. Each slide has a scene-graph/layer decision and uses the story lock for exact copy.
2. The calibration slide passes before batch reconstruction.
3. Every page scores at least 90/100 under `image-to-editable-reconstruction.md`; key pages score at least 94.
4. Ordinary text, tables, charts with source data, formulas, simple shapes, and page furniture are native/editable.
5. Retained images are separately selectable where feasible; no full-page reference image remains hidden underneath.
6. Registration-overlay review finds no major drift, ghost text, masking seam, or duplicated object.
7. Any unavoidable raster/editability exception is bounded and disclosed.

## Final checklist

- Titles are concise, high contrast, and do not wrap unexpectedly.
- Body text meets the intended projection/reading size.
- Cards contain complete text with adequate internal padding.
- Similar objects align and share dimensions.
- Red and navy encode meaning consistently.
- Charts have labels, units, legends/direct labels, and a takeaway.
- Tables use readable precision and do not overrun cells.
- Equations and symbols render correctly; all symbols are defined.
- Citations are readable and traceable.
- Footers, section labels, and page markers are correct.
- Top and bottom color blocks are not missing, reduced to hairlines, or detached from the slide edges.
- No source watermark, accidental branding, placeholders, or production notes remain.
- PPTX and PDF filenames clearly identify version.

For poster-led full-image mode, replace native-object editability checks with the dedicated gates in `poster-impact-mode.md`: exact wording, full-page visual integrity, consistent style, correct dimensions, and clean image-only assembly.
