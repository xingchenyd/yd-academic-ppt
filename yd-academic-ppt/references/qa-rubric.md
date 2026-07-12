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
| Technical integrity | Broken output | Minor conversion differences | Editable PPTX, faithful PDF, no clipping/overlap/placeholders |

## Required visual inspection

1. Render every PPTX slide to PNG.
2. Inspect every slide individually at full size.
3. Inspect a montage for pacing, repetition, and color balance.
4. Run overflow/slide-bound tests.
5. Export PDF and render representative PDF pages, including the densest slide, a chart/table slide, and the final slide.
6. Compare PPTX and PDF for fonts, line breaks, equations, charts, and page edges.

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
- No source watermark, accidental branding, placeholders, or production notes remain.
- PPTX and PDF filenames clearly identify version.

For poster-led full-image mode, replace native-object editability checks with the dedicated gates in `poster-impact-mode.md`: exact wording, full-page visual integrity, consistent style, correct dimensions, and clean image-only assembly.
