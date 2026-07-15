# yd-academic-ppt

`yd-academic-ppt` is a reusable Codex skill for creating polished academic, research, teaching, defense, journal-club, technical, policy, and formal professional presentations.

It first locks one outline and generates three complete ImageGen-led visual directions as full-deck contact-sheet images. After the user selects one, academic decks are reconstructed into highly faithful editable PowerPoint objects, while hackathon and creative decks retain the selected full-slide imagery for maximum impact. It then exports a matching PDF, asks targeted questions, and produces a refined second version.

## Core capabilities

- Argument-led presentation planning instead of mechanical document conversion.
- A formal default academic system built around warm off-white, deep navy, and restrained dark red.
- Template-fidelity calibration for the signature navy top banner, navy/red footer, numbered serif title lockup, rounded cards, compact editorial tables, and reference-like density.
- Automatic theme-led visual routing for hackathons, startups, games, coffee/food brands, cultural products, and other project pitches.
- Default pacing tiers of about 8 slides for 3 minutes, 12 for 5 minutes, and 20 for 10 minutes.
- Mandatory three-concept preview stage with one fixed storyline and three materially different, internally consistent visual systems.
- High-resolution contact-sheet PNG/JPEG previews containing every slide, delivered before any PPTX/PDF.
- Image-to-editable academic reconstruction using scene graphs, clean plates, separate visual assets, native text/tables/charts, registration overlays, and fidelity scoring.
- An explicit extreme poster mode that generates each entire 16:9 slide—including abundant artistic typography and dense coordinated elements—as one non-editable image.
- Adaptive layouts for definitions, literature reviews, methods, equations, charts, comparisons, workflows, cases, risks, synthesis, and conclusions.
- Editable academic text, tables, charts, formulas, simple diagrams, and separately movable image assets whenever practical.
- PPTX and PDF delivery for every version.
- Tailored post-draft questions and a disciplined version-two revision workflow.
- Full-slide rendering, overflow checks, readability checks, citation checks, and PPTX/PDF consistency QA.

## Structure

```text
yd-academic-ppt/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── academic-template-fidelity.md
    ├── design-system.md
    ├── duration-and-scenarios.md
    ├── evidence-and-research.md
    ├── image-to-editable-reconstruction.md
    ├── intake-and-iteration.md
    ├── layout-grammar.md
    ├── pitch-visual-systems.md
    ├── poster-impact-mode.md
    ├── qa-rubric.md
    ├── three-concept-preview.md
    ├── visual-generation-policy.md
    └── workflow.md
```

## Example invocation

```text
Use @yd-academic-ppt to turn these four papers into a 15-minute academic presentation. First lock the outline and generate three complete full-deck contact-sheet visual concepts without changing the storyline. Wait for my selection, reconstruct the selected academic design into a highly faithful editable PPTX, export PDF, then ask targeted questions before producing version 2.
```

The original visual reference screenshots are intentionally not included. The reusable design principles and workflow are encoded in the skill files without retaining source watermarks or branding.
