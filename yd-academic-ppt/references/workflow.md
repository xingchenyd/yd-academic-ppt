# End-to-end workflow: outline → three concepts → selection → V1 → V2

## 1. Frame the assignment

Extract or infer:

- Audience knowledge, role, and decision power.
- Occasion: classroom report, thesis defense, journal club, conference, training, proposal, executive briefing, or formal review.
- Speaking time and whether the file must also work as a standalone handout.
- Default page target: 8 slides for 3 minutes, 12 for 5 minutes, and 20 for 10 minutes unless the prompt overrides it.
- Topic boundary, required sections, forbidden content, language, institution, and author details.
- Source hierarchy: user files first, then authoritative external sources.
- Final deliverables: PPTX, PDF preview, notes, handout, or source appendix. Preliminary deliverables are the outline and three contact-sheet images.

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

## 3. Create and show the slide map

For every slide specify:

- Takeaway title.
- Audience question answered.
- Minimum evidence needed.
- Layout family.
- Visual emphasis.
- Estimated speaking time.

For the 3/5/10-minute defaults, design for a fast visual rhythm: many slides should advance in roughly 15–35 seconds, while a small number of core method, evidence, or demo slides may take 35–60 seconds. Cover, hook, transition, and closing pages may advance faster. For longer talks, derive a slower time ledger from the prompt. If the deck doubles as a handout, put detail in speaker notes or an appendix rather than shrinking body text.

Present this outline before image generation. Pause for confirmation unless the user explicitly authorized automatic continuation. Correct any structural issue, then freeze the story lock. All three visual concepts inherit it unchanged.

## 4. Prepare evidence and assets

Extract figures/tables from provided sources at adequate resolution. Preserve source data for later editable reconstruction. Maintain a private ledger connecting each claim or visual to its source.

## 5. Generate three complete concept decks

Follow `three-concept-preview.md`. Create three style bibles, validate cover/dense/data keyframes, then generate every slide for A/B/C. Build three deterministic contact sheets and verify that slide count/order/content are identical.

Deliver the outline, three boards, and a concise comparison. Pause for selection.

## 6. Build selected version 1

- Academic: follow `image-to-editable-reconstruction.md`; pass one dense calibration slide, then reconstruct the whole deck.
- Hackathon/creative/full-image: place each approved full-slide image edge-to-edge in PPTX; do not weaken it by partial generic reconstruction.
- Explicit editable creative pitch: use the academic reconstruction mechanics with the selected creative style bible.

Render every slide, inspect each at full size and as a montage, run overflow checks, export PDF, and compare PPTX/PDF. Apply `qa-rubric.md`.

## 7. Deliver and elicit

Deliver the selected-route PPTX and PDF preview together. Summarize important assumptions, reconstruction exceptions, or source limitations. Then ask 5–9 tailored questions and propose the highest-value improvements.

## 8. Produce version 2

Convert answers into a change ledger, resolve global changes first, then slide-specific changes. Preserve correct material. Re-render and re-run all QA; do not assume a small edit is layout-safe. Deliver both version-2 files and briefly summarize material improvements.
