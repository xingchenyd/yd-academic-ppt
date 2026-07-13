# yd-academic-ppt

`yd-academic-ppt` is a reusable Codex skill for creating polished academic, research, teaching, defense, journal-club, technical, policy, and formal professional presentations.

It turns topic descriptions, papers, datasets, notes, and existing decks into an editable PowerPoint presentation and a matching PDF preview. After the first version, it asks targeted questions and produces a refined second version.

## Core capabilities

- Argument-led presentation planning instead of mechanical document conversion.
- A formal default academic system built around warm off-white, deep navy, and restrained dark red.
- Template-fidelity calibration for the signature navy top banner, navy/red footer, numbered serif title lockup, rounded cards, compact editorial tables, and reference-like density.
- Automatic theme-led visual routing for hackathons, startups, games, coffee/food brands, cultural products, and other project pitches.
- Default pacing tiers of about 8 slides for 3 minutes, 12 for 5 minutes, and 20 for 10 minutes.
- Controlled image generation for text-free hero visuals and thematic assets, while ordinary presentation text remains editable.
- An explicit extreme poster mode that generates each entire 16:9 slide—including abundant artistic typography and dense coordinated elements—as one non-editable image.
- Adaptive layouts for definitions, literature reviews, methods, equations, charts, comparisons, workflows, cases, risks, synthesis, and conclusions.
- Editable text, tables, charts, formulas, and simple diagrams whenever practical.
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
    ├── intake-and-iteration.md
    ├── layout-grammar.md
    ├── pitch-visual-systems.md
    ├── poster-impact-mode.md
    ├── qa-rubric.md
    ├── visual-generation-policy.md
    └── workflow.md
```

## Example invocation

```text
Use @yd-academic-ppt to turn these four papers into a 15-minute academic presentation. Explain the research questions, models and methods, main conclusions, relationships among the papers, strengths, limitations, and possible improvements. Deliver an editable PPTX and PDF preview, then ask targeted questions before producing version 2.
```

The original visual reference screenshots are intentionally not included. The reusable design principles and workflow are encoded in the skill files without retaining source watermarks or branding.
