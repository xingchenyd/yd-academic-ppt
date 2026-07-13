---
name: yd-academic-ppt
description: "Create, redesign, or iteratively refine polished 16:9 academic, research, teaching, defense, journal-club, technical, policy, hackathon, startup, product-pitch, and formal professional PowerPoint decks. Default to the YD academic editorial style with warm off-white canvas, navy/red hierarchy, editable styled typography, modular evidence layouts, and rigorous QA; automatically switch to an editable theme-specific pitch system for games, coffee, cultural products, and startups, or an extreme non-editable full-image poster mode when the user explicitly requests complete ImageGen slides, abundant artistic lettering, or maximum promotional impact. Use when the user invokes yd-academic-ppt, supplies papers/data/notes for a deck, or requests PPTX/PDF output followed by targeted refinement."
---

# YD Academic PPT

Build a presentation as an argument, not a decorated document. Preserve the reference deck's disciplined hierarchy and editorial character while adapting composition to the subject.

## Required companion skills

Use the built-in `Presentations` skill for implementation and slide QA. Use the `pdf` skill to export and visually verify the PDF preview. Use `imagegen` only under the policy below. If the task requires current facts, citations, papers, or external visuals, research with authoritative sources before authoring.

Read these references before planning:

- [workflow.md](references/workflow.md) for the end-to-end two-version process.
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
2. Before version 1, ask only questions that block a credible deck, normally no more than three. Otherwise state assumptions briefly and proceed.
3. Create an audience-specific narrative and slide architecture before drawing slides.
4. Match the output contract to the selected route. Academic editorial and theme-led pitch routes build editable `.pptx` files with native text and data objects. Poster-led impact deliberately builds full-slide AI images and packages them into an image-based `.pptx`; no element-level editability is promised.
5. Export a matching `.pdf` preview and inspect both outputs.
6. Deliver version 1 with both files, then ask a tailored refinement questionnaire based on concrete uncertainties found during authoring.
7. After the user answers, revise the same deck into version 2, re-export the PDF, rerun full QA, and deliver both files. Avoid another broad questionnaire unless a new high-impact ambiguity appears.

## Mode routing

Choose one primary route before outlining:

- **Academic editorial — default:** use the reference-inspired warm off-white, navy, dark-red, structured-card system for academic reports, paper reviews, defenses, courses, formal reports, and unspecified topics. Unless the user requests a looser adaptation, treat this as **template-fidelity mode**: reproduce the signature top-left navy banner, top-right traits, bottom navy/red navigation band, numbered serif title lockup, red underline, rounded panels, and compact editorial tables on every applicable slide. Palette similarity alone is not sufficient.
- **Theme-led pitch:** trigger when the prompt indicates a hackathon, startup, product demo, game, coffee/food brand, cultural-tourism product, launch, campaign, or investor/judge pitch. Build a project-specific visual world instead of repainting the academic template.
- **Poster-led impact / full-image mode:** trigger only when the user explicitly asks for a promotional poster, image-generated full slides, extreme visual impact, a highly infectious hackathon pitch, dense poster composition, or abundant artistic lettering. Generate every slide as one complete 16:9 AI image containing the entire background, composition, illustration, typography, labels, diagrams, decorative elements, and page chrome. This mode intentionally sacrifices editability for maximum visual unity and impact.

Do not mix the academic chrome with a theme-led pitch unless the user explicitly wants a hybrid. Keep one coherent design language per deck. Read [poster-impact-mode.md](references/poster-impact-mode.md) whenever full-image mode triggers.

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

The first academic slide must be rendered as a **calibration slide** before the full deck is built. Compare it against [academic-template-fidelity.md](references/academic-template-fidelity.md). Do not proceed while any of these are missing: substantial top-left navy banner, full bottom navy/red band, serif title lockup, red underline, rounded card treatment, or reference-like information density.

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

- Image generation is allowed for text-free backgrounds, hero scenes, characters, product worlds, textures, decorative motifs, and thematic visual anchors.
- Generate visuals around planned text-safe areas. Add ordinary slide text afterward as native PowerPoint text.
- Do not ask an image model to render paragraphs, labels, tables, charts, citations, page numbers, or ordinary headings.
- In poster-led impact mode, permit extensive AI-rendered display lettering, short labels, badges, and integrated poster copy as part of the full-slide image. Follow the exact-copy and full-slide regeneration rules in [poster-impact-mode.md](references/poster-impact-mode.md).
- Use one dominant generated visual idea per slide, normally occupying one purposeful zone; do not scatter many unrelated generated stickers or images across the page.
- Keep charts, UI screenshots, paper figures, logos, and evidence faithful to their sources. Do not generate fake data, fake interfaces, or fake logos.

Follow [visual-generation-policy.md](references/visual-generation-policy.md) exactly.

## Version 1 procedure

1. Inspect all supplied files and images completely enough to understand content and visual constraints.
2. Write a private brief covering audience, occasion, duration/page target, required sections, evidence standard, editable-content needs, institutional identity, output language, mode route, typography direction, palette, image-generation allowance, logo policy, and pagination system.
3. Research only what is necessary; keep a source ledger.
4. Lock a private storyline and design system, then draft a storyboard containing slide number, takeaway title, purpose, evidence, layout family, visual anchor, native-text plan, image-generation need, and speaker-time estimate.
5. Check total timing and narrative gaps before implementation.
6. Implement with the `Presentations` skill using a reusable theme and layout helpers rather than one-off coordinates.
7. For the academic route, render one representative content slide first and pass the frame/title/component calibration gate. Then implement the remaining slides.
8. Render every slide, inspect full-size pages, fix layout defects, and export the PDF.
9. Run the rubric in [qa-rubric.md](references/qa-rubric.md), including the reference-fidelity comparison for academic decks.
10. Deliver both files and a concise summary of assumptions plus targeted refinement questions.

## Revision procedure

Translate the user's answers into a private change list grouped by content, structure, visual system, data/figures, and delivery context. Apply related changes globally, not page by page. Recheck cross-slide consistency after every structural change. Deliver version 2 as distinct filenames unless the user explicitly requests replacement.

## Non-negotiable quality gates

- No clipped, overlapping, off-canvas, or illegibly small content.
- No title wrapping unless the selected title layout explicitly supports two lines.
- No unsupported factual claim, invented citation, fabricated number, or unlabeled inference.
- No low-contrast gray body copy, washed-out fonts, or color-only meaning.
- No unresolved placeholders, watermarks, template-brand remnants, or accidental source branding.
- No screenshot of text when editable text can be used.
- No chart without units, labels, source/context, and an explicit takeaway.
- No PDF handoff before visual comparison with the PPTX render.

## Output naming

Use descriptive versioned names such as `<topic>_YD_V1.pptx`, `<topic>_YD_V1_preview.pdf`, `<topic>_YD_V2.pptx`, and `<topic>_YD_V2_preview.pdf`. Honor the user's filename when specified.
