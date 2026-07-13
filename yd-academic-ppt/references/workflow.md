# End-to-end workflow

## 1. Frame the assignment

Extract or infer:

- Audience knowledge, role, and decision power.
- Occasion: classroom report, thesis defense, journal club, conference, training, proposal, executive briefing, or formal review.
- Speaking time and whether the file must also work as a standalone handout.
- Default page target: 8 slides for 3 minutes, 12 for 5 minutes, and 20 for 10 minutes unless the prompt overrides it.
- Topic boundary, required sections, forbidden content, language, institution, and author details.
- Source hierarchy: user files first, then authoritative external sources.
- Deliverables: editable PPTX, PDF preview, notes, handout, or source appendix.

Ask at most three pre-build questions only if the missing answer changes the deck substantially. Otherwise record an assumption and proceed.

## 2. Build the message architecture

Write one deck thesis and one audience outcome. First choose academic editorial, theme-led pitch, or poster-led impact; then choose a narrative mode:

| Mode | Recommended spine |
| --- | --- |
| Academic study | Problem → gap → question → method → results → contribution → limitations |
| Multi-paper review | Shared problem → paper-by-paper evidence → comparison → relationship → critique → synthesis |
| Thesis defense | Motivation → research questions → technical route → studies/results → innovation → limits/future |
| Technical training | Mental model → building blocks → worked example → variants → decision rules → mistakes |
| Policy/proposal | Situation → evidence → options → evaluation → recommendation → implementation/risk |
| Executive report | Decision → evidence → implication → action → owner/timeline |
| Hackathon/product pitch | Hook → pain/opportunity → product promise → experience loop → proof/demo → differentiation → implementation → impact/ask |
| Game/creative project | World/premise → player/user problem → core loop → distinctive experience → system/technology → validation → roadmap |

Use section dividers only when they improve orientation. Keep background proportional to the audience's actual need.

## 3. Create the slide map

For every slide specify:

- Takeaway title.
- Audience question answered.
- Minimum evidence needed.
- Layout family.
- Visual emphasis.
- Estimated speaking time.

For the 3/5/10-minute defaults, design for a fast visual rhythm: many slides should advance in roughly 15–35 seconds, while a small number of core method, evidence, or demo slides may take 35–60 seconds. Cover, hook, transition, and closing pages may advance faster. For longer talks, derive a slower time ledger from the prompt. If the deck doubles as a handout, put detail in speaker notes or an appendix rather than shrinking body text.

## 4. Prepare evidence and assets

Extract figures/tables from provided sources at adequate resolution. Rebuild charts when the underlying data are available. Recreate simple diagrams with editable shapes; preserve complex scientific figures as images with clear citations. For theme-led pitches, generate only planned text-free hero visuals, backgrounds, characters, motifs, or product-world scenes, leaving intentional text-safe zones. Maintain a private ledger connecting each claim or visual to its source.

## 5. Author with a reusable system

Create global theme tokens, header/footer helpers, title treatments, card styles, table styles, chart colors, spacing constants, and page-number logic. Use these primitives consistently. Build central compositions from content needs rather than forcing a single repeated grid.

For the academic route, do not generate the full deck immediately. First build one representative dense calibration slide using `academic-template-fidelity.md`. Render it and verify the signature top banner, bottom band, title lockup, rounded components, table/card morphology, and content density. Freeze the corrected helpers only after this slide passes; then build the rest of the deck.

## 6. Validate version 1

Render every slide. Inspect each at full size and inspect a montage for rhythm. Run overflow checks. Export PDF, render the PDF, and compare representative slides against the PPTX render. For an academic deck, compare at least three full-size slides and the montage with `academic-template-fidelity.md`; missing frame elements or generic square/table styling require regeneration. Apply the full rubric in `qa-rubric.md`.

## 7. Deliver and elicit

Deliver the editable PPTX and PDF preview together. Summarize only important assumptions or source limitations. Then ask 5–9 tailored questions selected from `intake-and-iteration.md`; offer recommended defaults where useful.

## 8. Produce version 2

Convert answers into a change ledger, resolve global changes first, then slide-specific changes. Preserve correct material. Re-render and re-run all QA; do not assume a small edit is layout-safe. Deliver both version-2 files and briefly summarize material improvements.
