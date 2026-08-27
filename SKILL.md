---
name: pptx-code
description: Plan, generate, revise, and validate code-driven PowerPoint decks when narrative, evidence, charts, speaker notes, or layout fidelity matter. Use for .pptx creation or editing; skip when the user only wants a prose outline.
---

# PPTX Code

Make the deck help the audience understand the research, trust the evidence, and follow the speaker without reading dense prose.

## Plan the argument before the slides

- Establish the audience, speaking time, decision or research question, available evidence, and current visual baseline.
- Write the questions the audience is likely to ask. Order the deck as a continuous answer chain.
- Build a page map before coding. For each slide, record its job, short topic title, one-sentence takeaway, evidence, speaker-note purpose, and source.
- Keep an evidence ledger with period, sample, metric definition, benchmark, information cutoff, and source. A finished study may end with its conclusion and boundary; it does not need a forced next-step slide.
- When revising an existing deck, treat the user-approved or manually adjusted version as the visual baseline. Preserve unrelated edits and change only the requested surfaces.

## Give each slide one job

- Use a short topic phrase as the title. On ordinary content slides, add a conclusion subtitle that states the finding. Covers, agendas, section openers, and pure transitions may use a different hierarchy.
- Arrange three visual levels: takeaway, evidence, then source or qualification. Keep sources available without letting them compete with the result.
- Build evidence slides around one dominant visual. When the result can be shown as a chart, image, matrix, diagram, or compact table, let that visual occupy most of the usable page and move explanation into the takeaway and notes. Use SVG plus short text when no suitable chart or image exists; do not replace evidence with decorative imagery.
- Prefer charts for time, distribution, composition, and method comparison. Use tables for exact same-basis metrics, rules, and evidence records. Use text cards for no more than a few compact judgments.
- Label different periods and samples explicitly. Do not place incomparable numbers in one visual group.
- Explain enough method to answer why it was chosen, what problem it solves, how the rule works, and where it can fail. Technical novelty is useful only when it changes the inference.
- Turn weak or mixed results into a bounded research judgment: state where the evidence supports use, explanation, monitoring, or rejection.

## Write speaker notes as reasoning

- Point the audience to the relevant visual, name the evidence, explain the design choice or exception, state the conclusion, and connect to the next needed question.
- Keep notes aligned with what is visible, but do not read the slide aloud.
- Do not preview another slide after the final conclusion or at a completed study's endpoint.

## Implement with code

- Use the repository's existing presentation library, helper functions, assets, and template when available.
- Keep reusable code free of personal absolute paths, credentials, and project data. Resolve project assets from the script or repository root.
- Put a multi-project deck and its generator at the shared project level unless the user specifies another location.
- Use real analysis outputs for charts. Keep source files and metric definitions traceable.
- Use a legible font system. Default body text to at least 22 pt unless the user or template specifies otherwise; citations and footers may be smaller.
- Integrate generated figures with the slide palette. For Matplotlib charts placed directly on a page, set the figure, axes, and exported image background to the slide background color. When the chart needs separation, use an intentional same-palette tint or card instead of the library's default white canvas. Keep transparency only when the target renderer has been verified.
- Store speaker notes in the PPTX rather than in a separate file unless the user requests both.

## Validate the delivered file

1. Generate the deck from a clean invocation and reopen the saved PPTX.
2. Run `scripts/validate_pptx.py` for deterministic checks. Treat its geometry and capacity findings as review leads, not rendered truth.
3. Render with an installed PowerPoint-compatible application and inspect the actual pages. Check overflow, overlap, line breaks, chart proportions, table density, font substitution, SVG distortion, image borders or background seams, page numbers, notes, and animation residue.
4. If rendering is unavailable, say so. Do not claim visual inspection from code checks alone.
5. Read back the final output path, slide count, titles, notes coverage, and validation result after any generator or office application changes the file.

For the detailed research-deck workflow and slide-selection rules, read [references/research-ppt-workflow.md](references/research-ppt-workflow.md).

Run the validator with:

```bash
python scripts/validate_pptx.py path/to/deck.pptx --require-notes --min-font 22
```
