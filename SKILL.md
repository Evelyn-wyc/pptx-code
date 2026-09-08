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
- Separate internal provenance from visible citations. Keep local filenames, data paths, notebook cells, and generated artifacts in the evidence ledger or notes for reproducibility; do not print them as slide citations unless the audience needs the path for an audit or handoff. Reserve ordinary visible source lines for literature, webpages, external datasets, and other published material.
- When revising an existing deck, treat the user-approved or manually adjusted version as the visual baseline. Preserve unrelated edits and change only the requested surfaces.
- For a mixed-domain audience, identify the concepts that need a plain-language definition or one stable analogy. Use the analogy to establish intuition, then return to the real technical labels; do not spread metaphor-specific terminology across the whole deck.
- Allocate spoken detail by importance. Keep implementation parameters, derivations, and exact secondary metrics available for questions without forcing them into the main presentation path.

## Establish the template and font contract

- This skill does not provide a default PowerPoint template or visual style. Use a template supplied by the user, or have the user specify the intended visual direction before authoring. Do not silently substitute an unrelated stock template or describe an inferred design as official.
- Treat a supplied template as presentation structure, not only as a background image. Inspect its slide masters, layouts, theme, placeholders, footer behavior, and example slides. When it contains several designs, identify the selected design by its master and layout rather than assuming that a slide number is the template identity. Keep generated slides on that design unless a deliberate section change calls for another one.
- Establish the target operating systems and presentation applications before choosing fonts. Specify Latin and East Asian typefaces separately, and use fonts available in every required environment or record an explicit installation or substitution plan. Do not rely on automatic CJK fallback for layout-critical text.
- When the presentation library permits it, write both Latin and East Asian typeface settings into the PPTX. Size text boxes against the intended typefaces rather than an exact measured fit. For ordinary CJK or mixed CJK/Latin text, leave unused horizontal width equivalent to at least two full-width Chinese characters (`2 em`) on each intended line after margins; reserve a comparable `2 em` for other scripts. Use intentional line breaks so that small metric differences between font implementations do not change the hierarchy or create orphaned lines. If the reserve does not fit, widen the box or rewrite the copy before reducing font size; do not treat AutoFit or shrink-on-overflow as the reserve.

## Give each slide one job

- Use a short topic phrase as the title. On ordinary content slides, add a conclusion subtitle that states the finding. Covers, agendas, section openers, and pure transitions may use a different hierarchy.
- Prefer concrete subject-verb conclusions over abstract nominal phrases. Replace unexplained terms such as `regime resilience`, `estimation risk`, or `changing universe` with the observed object and action, or define the technical term on first use.
- Do not repeat the same conclusion in the title, subtitle, chart annotation, and a separate insight card. If the title already carries the finding, use the freed space to enlarge the evidence; omit a subtitle when it adds no new information.
- Arrange three visual levels: takeaway, evidence, then source or qualification. Keep sources available without letting them compete with the result.
- Use covers to identify the topic, speaker, and affiliation. Put result metrics on the cover only when the audience and use case call for an executive-summary opening.
- Build evidence slides around one dominant visual. When the result can be shown as a chart, image, matrix, diagram, or compact table, let that visual occupy most of the usable page and move explanation into the takeaway and notes. Use SVG plus short text when no suitable chart or image exists; do not replace evidence with decorative imagery.
- Give each evidence visual one analytical job. Do not repeat the same chart on multiple slides unless the annotation, comparison basis, or question changes materially; redraw or choose a different view when the second slide needs different evidence.
- Prefer charts for time, distribution, composition, and method comparison. Use tables for exact same-basis metrics, rules, and evidence records. Use text cards for no more than a few compact judgments.
- Make every evidence visual self-contained. Label axes, units, periods, samples, colors, marker shapes, line styles, and comparison groups; define abbreviations and symbols at first use. If a figure contains padding, missingness, aggregation, or transformed values, state what is included, excluded, or encoded.
- When several callout boxes make the primary chart too small, remove repeated prose and place one concise annotation or legend inside the enlarged chart.
- Label different periods and samples explicitly. Do not place incomparable numbers in one visual group.
- For controlled or factorial experiments, show which input and model dimensions change, what stays fixed, and every comparison needed to support the component claim. Group contrasts by component so the audience can see the direction and basis without reconstructing the design mentally.
- Explain enough method to answer why it was chosen, what problem it solves, how the rule works, and where it can fail. Technical novelty is useful only when it changes the inference.
- Turn weak or mixed results into a bounded research judgment: state where the evidence supports use, explanation, monitoring, or rejection.
- Match claim strength to the displayed evidence. Describe a point estimate as an observed gain; do not call a result significant, robust, or inconclusive unless the slide or notes provide the uncertainty, repeated-fit, or sensitivity evidence needed for that statement.
- Connect technical evidence to domain meaning in plain language, but keep the interpretation no stronger than the experiment. A financial or operational insight should explain what the result means, not restate the metric with different jargon.
- Treat every non-appendix slide as part of the spoken path. Add an appendix only when the presentation format and user intent make some material genuinely optional for delivery.
- End a completed study with the selected method, the minimum decisive metrics, and one concrete conclusion. Do not repeat the full architecture, training recipe, and experiment history on the final slide.

## Write speaker notes as reasoning

- Point the audience to the relevant visual, name the evidence, explain the design choice or exception, state the conclusion, and connect to the next needed question.
- Follow the visual reading order, normally left to right and top to bottom. Use short pointing cues so the spoken sequence and the audience's gaze stay synchronized.
- Keep notes aligned with visible wording. Reuse or briefly read concise labels and takeaways when that helps the speaker recover the thread, but do not mechanically recite dense slide copy.
- Do not preview another slide after the final conclusion or at a completed study's endpoint.
- Write notes as spoken language rather than report prose. Explain displayed equations in words instead of reproducing notation in the script, and define any necessary symbols next to the equation on the slide.
- Keep each slide's script concise. Prefer short paragraphs in which one to three sentences explain one idea.
- Reuse the slide's visible terms, labels, and conclusion wording where natural, so the speaker can recover the thread by looking at the page.
- When the visual already carries exact values, let the audience read them. State the direction, relative size, comparison, and conclusion instead of speaking a sequence of small decimals; read only the few headline values that matter, using sensible rounding when exact precision is not part of the claim.
- When a figure carries the explanation, use the notes to identify its axes and marks, explain the comparison, and state the takeaway. Do not duplicate every label or narrate every point.
- Build the explanation from first principles: state what was done, why that choice follows from the problem, and what the evidence means.
- Emphasize the implemented design and observed result. Avoid defensive lists of absent components or repeated `we do not` phrasing unless an exclusion is necessary to define validity, safety, compatibility, or the evidence boundary.
- For bilingual scripts, choose one language as the source of truth, keep language sections in a consistent order, and translate slide by slide so the two versions preserve the same claims, paragraph structure, and emphasis.
- For code-generated decks, keep the slide-aligned script in the generator or in one source file consumed by it, write the script into PPTX speaker notes during the build, and validate note coverage after saving.

## Implement with code

- Use the repository's existing presentation library, helper functions, assets, and template when available.
- Keep reusable code free of personal absolute paths, credentials, and project data. Resolve project assets from the script or repository root.
- Put a multi-project deck and its generator at the shared project level unless the user specifies another location.
- Use real analysis outputs for charts. Keep source files and metric definitions traceable.
- Use a legible font system. Default body text to at least 22 pt unless the user or template specifies otherwise; citations and footers may be smaller.
- Use a PowerPoint slide-number field in the footer when pages are numbered, rather than hard-coded numerals. Covers may omit the field when the design calls for it. Verify numbering after slides are inserted, removed, or reordered.
- Integrate generated figures with the slide palette. For Matplotlib charts placed directly on a page, set the figure, axes, and exported image background to the slide background color. When the chart needs separation, use an intentional same-palette tint or card instead of the library's default white canvas. Keep transparency only when the target renderer has been verified.
- Use the same terminology for a concept in the slide, chart, legend, and notes. Spell out an abbreviation at first use, then use one short form consistently.
- Store speaker notes in the PPTX rather than in a separate file unless the user requests both.

## Validate the delivered file

1. Generate the deck from a clean invocation and reopen the saved PPTX.
2. Run `scripts/validate_pptx.py` for deterministic checks. Treat its geometry and capacity findings as review leads, not rendered truth.
3. Render with an installed PowerPoint-compatible application and inspect the actual pages. Check overflow, overlap, line breaks, chart proportions, table density, font substitution, SVG distortion, image borders or background seams, page numbers, notes, visible spell-check underlines, and animation residue. Confirm that legends, axes, units, symbols, abbreviations, and comparison groups remain legible at presentation scale. Look specifically for orphaned final lines containing only one word, one or two CJK characters, or another short fragment. Also flag lines that fit in the current renderer but have less than the required `2 em` horizontal reserve. Rewrite or widen the text box before reducing font size, unless the short line is an intentional display treatment.
4. When cross-platform fidelity is required, render with every accessible target application or operating system and compare the resulting pages. A successful render in LibreOffice, Keynote, or a browser viewer does not by itself prove parity with Microsoft PowerPoint. If a required environment is unavailable, name the unverified environment and do not claim full cross-platform validation; provide a PDF preview when it helps the user perform the remaining check.
5. Review information duplication after rendering. Remove repeated takeaway boxes or secondary prose that shrinks the primary evidence without adding a distinct claim.
6. If rendering is unavailable, say so. Do not claim visual inspection from code checks alone.
7. Read back the final output path, slide count, titles, notes coverage, and validation result after any generator or office application changes the file.

For the detailed research-deck workflow and slide-selection rules, read [references/research-ppt-workflow.md](references/research-ppt-workflow.md).

Run the validator with:

```bash
python scripts/validate_pptx.py path/to/deck.pptx --require-notes --min-font 22
```
