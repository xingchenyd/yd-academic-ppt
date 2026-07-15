---
name: yd-academic-ppt
description: "Create, redesign, or iteratively refine polished 16:9 academic, research, teaching, defense, journal-club, technical, policy, hackathon, startup, product-pitch, and formal professional decks through a three-concept visual workflow. First lock one outline and storyline, then use ImageGen to produce three complete full-deck contact-sheet previews in distinct but internally consistent visual systems. After the user selects one, reconstruct academic decks into highly faithful editable PPTX objects, or assemble creative/hackathon full-slide images directly into PPTX; export PDF, ask targeted questions, and produce a refined version 2. Use when the user invokes yd-academic-ppt, supplies papers/data/notes, asks for multiple visual directions, or requests PPTX/PDF delivery."
---

# YD Academic PPT

Build a presentation as an argument, not a decorated document. Preserve the reference deck's disciplined hierarchy and editorial character while adapting composition to the subject.

## Required companion skills

Use the built-in `Presentations` skill for implementation and slide QA. Use the `pdf` skill to export and visually verify the PDF preview. Use `imagegen` only under the policy below. If the task requires current facts, citations, papers, or external visuals, research with authoritative sources before authoring.

Read these references before planning:

- [workflow.md](references/workflow.md) for the end-to-end two-version process.
- [three-concept-preview.md](references/three-concept-preview.md) for the mandatory outline lock and three full-deck contact-sheet previews.
- [image-to-editable-reconstruction.md](references/image-to-editable-reconstruction.md) after an academic preview direction is selected.
- [design-system.md](references/design-system.md) for visual tokens and typography.
- [academic-template-fidelity.md](references/academic-template-fidelity.md) whenever the academic editorial route is selected; it defines the mandatory frame, title anatomy, rounded components, table construction, and visual comparison gates distilled from the reference images.
- [layout-grammar.md](references/layout-grammar.md) for page archetypes and density rules.
- [intake-and-iteration.md](references/intake-and-iteration.md) for questions and revision logic.
- [qa-rubric.md](references/qa-rubric.md) before each delivery.
- [evidence-and-research.md](references/evidence-and-research.md) when claims, papers, data, or sources matter.
- [duration-and-scenarios.md](references/duration-and-scenarios.md) to select page count and narrative structure.
- [visual-generation-policy.md](references/visual-generation-policy.md) before generating any image or stylized title.
- [pitch-visual-systems.md](references/pitch-visual-systems.md) for hackathons, startups, games, coffee, cultural products, and other theme-led decks.

## Operating contract

1. Infer as much as possible from the user's prompt and source files. Do not make the user restate information already available.
2. Before visual generation, ask only questions that block a credible outline, normally no more than three. Otherwise state assumptions briefly and proceed.
3. Present the outline/slide map first. Lock one audience-specific narrative, exact slide order, takeaway titles, claims, data, evidence, and timing ledger. Pause for outline confirmation unless the user has explicitly authorized automatic continuation.
4. After outline confirmation and before any PPTX or PDF, generate **three complete full-deck visual concepts** from that same story lock and deliver three contact-sheet images—one image per concept containing every slide in order. These are PNG/JPEG preview boards, not PDF files.
5. Pause for the user's A/B/C selection or a precise hybrid instruction. Do not silently choose a direction and continue.
6. Match the selected route: academic decks are reconstructed from the approved full-slide images into highly faithful editable native objects; hackathon/poster/high-impact creative decks keep the approved full-slide images and assemble them directly into PPTX. An editable creative pitch is an explicit exception.
7. Export a matching `.pdf` only after the selected formal PPTX is built, inspect both outputs, and deliver version 1.
8. Ask a tailored refinement questionnaire and propose concrete improvements. After the user answers, revise into version 2, re-export PDF, rerun full QA, and deliver both files.

## Mode routing

Choose one primary route before outlining:

- **Academic editorial — default:** use the reference-inspired warm off-white, navy, dark-red, structured-card system for academic reports, paper reviews, defenses, courses, formal reports, and unspecified topics. Unless the user requests a looser adaptation, treat this as **template-fidelity mode**: reproduce the signature top-left navy banner, top-right traits, bottom navy/red navigation band, numbered serif title lockup, red underline, rounded panels, and compact editorial tables on every applicable slide. Palette similarity alone is not sufficient.
- **Creative pitch / hackathon — image-based by default:** for hackathons, game concepts, creative products, campaigns, coffee/food brands, cultural-tourism products, launches, and high-energy judge pitches, build a project-specific visual world. After selection, assemble the approved full-slide images directly into PPTX for maximum unity and impact. Reconstruct into editable objects only when the user explicitly prioritizes editability.
- **Poster-led impact / extreme full-image mode:** trigger when the user requests promotional-poster intensity, abundant artistic lettering, dense visual layering, or maximum stage impact. It uses the same three-concept selection stage but pushes ImageGen density and art direction further.

Do not mix the academic chrome with a creative pitch unless the user explicitly wants a hybrid. Keep one coherent design language per concept and deck. Read [poster-impact-mode.md](references/poster-impact-mode.md) for creative image-based output.

## Duration defaults

If the user specifies only time and not page count, use these defaults including cover and closing pages:

- 3 minutes → about 8 slides.
- 5 minutes → about 12 slides.
- 10 minutes → about 20 slides.

If the user says the talk is longer, supplies a page count, or gives a content-heavy brief, derive the count from the prompt rather than extrapolating mechanically. Follow [duration-and-scenarios.md](references/duration-and-scenarios.md).

## Narrative rules

- Define one governing sentence for the deck: what the audience should believe, understand, or decide afterward.
- Give every slide one job and one takeaway. Prefer conclusion-style titles; use topic titles only for section dividers or foundational definitions.
- Make the title sequence readable as a compact outline of the argument.
- Build evidence chains: context/problem → question → approach → evidence → interpretation → implication → limitations/next step.
- Separate the user's requested content from internal planning. Never expose production notes on visible slides.
- Do not copy a paper's section order mechanically. Reorder content for the audience and speaking time.
- Use repetition intentionally: stable header/footer chrome, section markers, numbering, and takeaway strips; vary the central composition to match the content.
- Prefer meaningful compression over tiny text. Split a slide when two independent claims compete.

## YD visual identity

Treat the reference style as the default academic editorial system with a stable frame and flexible center:

- Use a warm off-white canvas, deep navy as the structural color, restrained dark red for contrast and decisions, and a small amount of muted gold only when appropriate.
- Use large, high-contrast navy Chinese **serif** titles by default, with a compact numbered badge aligned to the title baseline and a short, thick red underline/accent. A generic sans title is a deliberate exception, not the default.
- Use thin borders, visibly rounded cards, flat fills, precise alignment, and consistent circular icon containers. Avoid square dashboard boxes, gradients, glass effects, neon, excessive shadows, and decorative stock imagery.
- Keep the signature top and bottom color-block frame on normal academic slides. Remove or replace it only when the user supplies an institution template or explicitly requests a frameless/conference style.
- Use cards for distinct semantic units, not as automatic decoration. A slide may be flat, chart-led, figure-led, or table-led when that communicates better.
- Use navy/red alternation to encode category, contrast, sequence, or risk—not merely to add color.
- Never fall back to plain black Song type as the visible design system. Use theme-appropriate font families, weights, colors, emphasis, and spacing. Academic serif titles may be used only when deliberately styled in navy/red with strong weight and hierarchy; body copy should normally use a clean sans-serif Chinese font.

Follow the exact tokens and exceptions in [design-system.md](references/design-system.md).

For the academic route, the three ImageGen concepts are the visual exploration stage. After selection, reconstruct one representative dense slide as a **calibration slide** before rebuilding the remaining pages. Compare it with the selected full-slide image and [academic-template-fidelity.md](references/academic-template-fidelity.md). Do not proceed while the silhouette, frame, title anatomy, rounded components, table morphology, typography, or density visibly drift.

## Content-to-layout routing

Select the smallest useful layout family from [layout-grammar.md](references/layout-grammar.md):

- Definition or thesis → dominant claim plus 2–3 supporting blocks.
- Literature/paper review → research question, method/model, evidence, finding, contribution, limitation, and cross-paper linkage.
- Method/model → staged pipeline, architecture, equation with variable legend, or input–process–output layout.
- Numeric result → chart or table with a highlighted inference and source.
- Comparison → aligned two-column or matrix layout with identical dimensions.
- Process/workflow → numbered stages with decisions and feedback loops.
- Case/example → setup, calculation/evidence, result, and interpretation.
- Risk/limitations → categorized warning cards plus mitigation or improvement path.
- Synthesis → relationship map, shared mechanism, disagreement, gap, and proposed direction.
- Conclusion → 3–5 memorable claims, not a transcript of the deck.

Avoid repeating the same silhouette on more than two consecutive content slides unless a deliberate series comparison requires it.

## Image and text policy

- At concept stage, use ImageGen for complete 16:9 slide compositions in all three routes. Read [three-concept-preview.md](references/three-concept-preview.md).
- For academic concept boards, ImageGen controls the entire visual composition; exact factual text may be added as a rasterized overlay after generation so titles, claims, symbols, and numbers remain correct. Do not treat AI-rendered microtext as evidence.
- After academic selection, use the approved images only as visual targets. Rebuild ordinary text, tables, charts, formulas, lines, simple geometry, page furniture, and data-bound objects natively. Retain complex illustration/photo/texture regions as separately movable image assets when native reconstruction would reduce fidelity.
- In poster-led impact mode, permit extensive AI-rendered display lettering, short labels, badges, and integrated poster copy as part of the full-slide image. Follow the exact-copy and full-slide regeneration rules in [poster-impact-mode.md](references/poster-impact-mode.md).
- Use one dominant generated visual idea per slide, normally occupying one purposeful zone; do not scatter many unrelated generated stickers or images across the page.
- Keep charts, UI screenshots, paper figures, logos, and evidence faithful to their sources. Do not generate fake data, fake interfaces, or fake logos.

Follow [visual-generation-policy.md](references/visual-generation-policy.md) exactly.

## Concept-selection and version 1 procedure

1. Inspect all supplied files and images completely enough to understand content and visual constraints.
2. Write a private brief covering audience, occasion, duration/page target, required sections, evidence standard, editable-content needs, institutional identity, output language, mode route, typography direction, palette, image-generation allowance, logo policy, and pagination system.
3. Research only what is necessary; keep a source ledger.
4. Produce and show the outline/slide map. Pause for confirmation unless the user already said to proceed automatically; lock the story after correcting any issue.
5. Create three materially distinct style bibles while holding the story lock fixed. Generate every slide for A, B, and C, then compose three full-deck contact-sheet images. Run the concept-board QA and deliver the three boards plus a concise difference table.
6. Wait for selection. If the user requests a hybrid, state exactly which attributes come from which concept and keep one coherent final system.
7. For academic output, follow [image-to-editable-reconstruction.md](references/image-to-editable-reconstruction.md), pass a one-slide calibration, then rebuild all slides. For creative/hackathon output, place each approved full-slide image edge-to-edge in PPTX.
8. Render every slide, inspect full-size pages and montage, run technical/fidelity QA, and export the PDF.
9. Deliver version 1 PPTX + PDF, then ask targeted questions and propose high-value improvements.
10. Apply the answers to version 2, rerun complete QA, and deliver PPTX + PDF.

## Revision procedure

Translate the user's answers into a private change list grouped by content, structure, visual system, data/figures, and delivery context. Apply related changes globally, not page by page. Recheck cross-slide consistency after every structural change. Deliver version 2 as distinct filenames unless the user explicitly requests replacement.

## Non-negotiable quality gates

- No clipped, overlapping, off-canvas, or illegibly small content.
- No title wrapping unless the selected title layout explicitly supports two lines.
- No unsupported factual claim, invented citation, fabricated number, or unlabeled inference.
- No low-contrast gray body copy, washed-out fonts, or color-only meaning.
- No unresolved placeholders, watermarks, template-brand remnants, or accidental source branding.
- In the final academic deck, no screenshot of ordinary text, tables, charts, formulas, or simple shapes when they can be rebuilt editably without meaningful fidelity loss.
- No chart without units, labels, source/context, and an explicit takeaway.
- No PDF handoff before visual comparison with the PPTX render.

## Output naming

Use `<topic>_outline.txt`, `<topic>_concept_A_contactsheet.png`, `<topic>_concept_B_contactsheet.png`, and `<topic>_concept_C_contactsheet.png` before selection. After selection use `<topic>_YD_V1.pptx`, `<topic>_YD_V1_preview.pdf`, `<topic>_YD_V2.pptx`, and `<topic>_YD_V2_preview.pdf`. Honor the user's filename when specified.
