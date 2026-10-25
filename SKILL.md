---
name: pptx-code
description: Plan, generate, revise, and validate code-driven PowerPoint decks when narrative, evidence, charts, speaker notes, or layout fidelity matter. Use for .pptx creation or editing; skip when the user only wants a prose outline.
---

# PPTX Code

Make the deck help the audience understand the research, trust the evidence, and follow the speaker without reading dense prose.

The presentation defaults below reflect this user's recurring preferences. Apply them to new or revised content unless the current brief explicitly specifies otherwise; preserve approved content outside the requested scope. Keep project-specific palettes, font families, filenames, environments, and page counts in the project rather than making them universal skill requirements.

## Plan the argument before the slides

- Establish the audience, speaking time, decision or research question, available evidence, and current visual baseline.
- Before slide construction, have the author or the assisting AI organize the completed work into an argument. For each experiment or activity, identify the question or observed phenomenon it addresses, why that comparison is informative, its evidence, and what its result changes. Review the logical sequence before coding; this can be an AI self-review within the authorized task and does not itself require another approval round.
- Order the presentation as a continuous answer chain: question → reason for the test → evidence → interpretation → next unresolved question or final decision. Let logical dependencies determine the order rather than the chronology of experiments, available chart files, or model complexity. Preserve the distinction between an original hypothesis and a retrospective explanation; do not invent a preplanned motive for exploratory work.
- Build a page map before coding. For each slide, record its question, why the experiment belongs here, short topic title, one-sentence takeaway, evidence, connection to the next question, speaker-note purpose, and source. The takeaway is an internal planning statement, not an instruction to add a subtitle. Construction starts after this map passes the logic review; every experiment on the spoken path must have an identifiable role.
- Keep an evidence ledger with period, sample, metric definition, benchmark, information cutoff, and source. A finished study may end with its conclusion and boundary; it does not need a forced next-step slide.
- Separate internal provenance from visible citations and spoken notes. Keep local filenames, data paths, notebook cells, timing estimates, and build records in the evidence ledger or existing audit assets. Use compact, standard bibliographic citations for papers in a consistent source band; a bare URL or blue hyperlink is not a complete paper citation. Web sources can use descriptive titles and links where appropriate.
- When revising an existing deck, treat the latest saved user-approved or manually adjusted version as the baseline for both content and appearance. Inspect it before rebuilding, preserve unrelated edits, and update the generator to reproduce the revised version. Respect a requested output suffix or separate generated copy.
- For a mixed-domain audience, identify the concepts that need a plain-language definition or one stable analogy. Use the analogy to establish intuition, then return to the real technical labels; do not spread metaphor-specific terminology across the whole deck.
- Allocate pages and spoken detail to the actual time limit and importance of each result. Keep implementation parameters, derivations, and exact secondary metrics available for questions without forcing them into the main presentation path.

## Establish the template and font contract

- This skill does not provide a default PowerPoint template or visual style. Use a template supplied by the user, or have the user specify the intended visual direction before authoring. Do not silently substitute an unrelated stock template or describe an inferred design as official.
- Treat a supplied template as presentation structure, not only as a background image. Inspect its slide masters, layouts, theme, placeholders, footer behavior, and example slides. When it contains several designs, identify the selected design by its master and layout rather than assuming that a slide number is the template identity. Keep generated slides on that design unless a deliberate section change calls for another one.
- Preserve the appearance the user approved, including typeface, weight, and density. Inspect a rendered baseline as well as its declared font names: a substituted font can be the appearance the user intended. Resolve the visible typeface into an explicit font choice and verify it in the target application; retaining a font name alone does not establish visual continuity.
- Use large, visibly strong type: ordinary content titles should share one size, weight, and position, normally 30–32 pt bold; authored body text and key chart labels should normally be at least 22 pt, using bold or semibold. References and secondary captions may use 18 pt; template footers may be smaller. Resolve the actual font weight rather than relying on a nominal `bold` flag. Enlarge or simplify content before reducing type size. Check text inside SVGs and raster figures at its final slide scale as well as native text boxes.
- Use dark, high-contrast text for substantive content. Keep comparable findings equally readable rather than making some pale gray or a faint theme tint. Extend the approved palette with a few coordinated accents. Prefer light content backgrounds; use dark panels only when the approved design calls for them.
- Establish the target operating systems and presentation applications before choosing fonts. Specify Latin and East Asian typefaces separately, and use fonts available in every required environment or record an explicit installation or substitution plan. Do not rely on automatic CJK fallback for layout-critical text.
- When the presentation library permits it, write both Latin and East Asian typeface settings into the PPTX. Size text boxes against the intended typefaces rather than an exact measured fit. For ordinary CJK or mixed CJK/Latin text, leave unused horizontal width equivalent to at least two full-width Chinese characters (`2 em`) on each intended line after margins; reserve a comparable `2 em` for other scripts. Use intentional line breaks so that small metric differences between font implementations do not change the hierarchy or create orphaned lines. If the reserve does not fit, widen the box or rewrite the copy before reducing font size; do not treat AutoFit or shrink-on-overflow as the reserve.
- Leave visible internal padding on all sides of cards and text boxes, plus vertical room for line spacing, paragraph spacing, and font substitution. Keep text comfortably inside its frame; do not solve a fit problem by squeezing margins to zero.

## Give each slide one job

- Use a short, informative topic title. Do not add a one-sentence summary or conclusion subtitle beneath it unless explicitly requested. Avoid decorative eyebrow labels or prefixes such as `SELF`, `Research`, or `Part I`; maintain any needed navigation through PowerPoint sections or dedicated section slides. A title should identify the page's subject without becoming a long sentence or an opaque one-word label.
- Prefer concrete subject-verb conclusions over abstract nominal phrases. Replace unexplained terms such as `regime resilience`, `estimation risk`, or `changing universe` with the observed object and action, or define the technical term on first use.
- Let the evidence and spoken explanation carry the conclusion. Add a brief annotation beside the relevant data only when it helps interpretation; do not repeat the finding in a title, banner, and separate insight card.
- Arrange three visual levels: topic title, dominant evidence, then source or qualification. Keep sources available without letting them compete with the result.
- Center the complete body composition within the usable content region, both vertically and horizontally. Its upper edge is below the title separator when present (otherwise below the approved header block); its lower edge is above the footer or fixed source band. Its left and right edges are the template's content margins. Balance the visible space around the combined chart, labels, tables, cards, and body copy while preserving useful internal alignments. Left-aligned text can belong to a centered composition. Use rendered content bounds rather than the slide center or an image's padded canvas; see the [body-region procedure](references/research-ppt-workflow.md#body-region-layout).
- Use covers to identify the topic, speaker, and affiliation. Put result metrics on the cover only when the audience and use case call for an executive-summary opening.
- Build evidence slides around a dominant chart, figure, diagram, or coherent set of panels. Keep visible prose to short labels and essential annotations; move the explanation into spoken notes. Several related plots can share a page when each remains legible and their comparison answers one question.
- Reuse suitable original paper figures and presentation assets first. Locate source images through the original PPT, HTML asset references, or figure files before taking screenshots of rendered pages. Preserve resolution and scientific meaning; crop, enlarge, or rearrange panels when needed for legibility. Use native diagrams or SVGs for a missing conceptual explanation, with labels sized for the final slide; do not redraw existing research evidence merely to restyle it.
- Give each evidence visual one analytical job. Do not repeat the same chart on multiple slides unless the annotation, comparison basis, or question changes materially; redraw or choose a different view when the second slide needs different evidence.
- Prefer charts for time, distribution, composition, and method comparison. Use tables for exact same-basis metrics, rules, and evidence records. Use text cards for a few compact judgments, not as the repeated layout for every page. Merge sparse neighboring slides when they address the same question and the combined evidence stays readable; split dense pages by argumentative job.
- Make every evidence visual self-contained. Label axes, units, periods, samples, colors, marker shapes, line styles, and comparison groups; define abbreviations and symbols at first use. If a figure contains padding, missingness, aggregation, or transformed values, state what is included, excluded, or encoded.
- When several callout boxes make the primary chart too small, remove repeated prose and place one concise annotation or legend inside the enlarged chart.
- Label different periods and samples explicitly. Do not place incomparable numbers in one visual group.
- For controlled or factorial experiments, show which input and model dimensions change, what stays fixed, and every comparison needed to support the component claim. Group contrasts by component so the audience can see the direction and basis without reconstructing the design mentally.
- Explain enough method to answer why it was chosen, what problem it solves, how the rule works, and where it can fail. Technical novelty is useful only when it changes the inference.
- Turn weak or mixed results into a bounded research judgment: state where the evidence supports use, explanation, monitoring, or rejection.
- Match claim strength to the displayed evidence. Describe a point estimate as an observed gain; do not call a result significant, robust, or inconclusive unless the slide or notes provide the uncertainty, repeated-fit, or sensitivity evidence needed for that statement.
- Connect technical evidence to domain meaning in plain language, but keep the interpretation no stronger than the experiment. A financial or operational insight should explain what the result means, not restate the metric with different jargon.
- Treat every non-appendix slide as part of the spoken path. Add an appendix only when the presentation format and user intent make some material genuinely optional for delivery.
- End a completed study by restating the contribution and the few decisive results, including efficiency or cost when supported. A concise text layout or a few light cards is appropriate; do not repeat a previously shown figure merely to fill the conclusion page.

## Use native mathematical equations

- Put displayed mathematical expressions in PowerPoint's native equation environment, equivalent to inserting an equation with `Alt+=`. In code-generated PPTX files use Office Math (OMML), with structural fractions, subscripts, superscripts, sums, roots, and matrices where the expression requires them. Ordinary text, Unicode lookalikes, or a formula image alone do not fulfill native equation editability.
- Keep explanatory prose outside the math object and use the established body font for that prose. Use a supported math font for mathematical symbols. Define each symbol and index before or next to its first equation; explain in the notes what the formula computes and why that calculation answers the research question.
- Retain one authoritative expression for native output and any compatibility fallback. If a renderer needs a fallback, package it as alternate content rather than a second visible equation. Check mathematical equivalence of both branches, especially index scope, minus signs, limits, and denominators.
- Validate the saved package for real Office Math objects and inspect the equations rendered by Microsoft PowerPoint whenever it is accessible. Check structure, legibility, bounds, and inline alignment; the mere presence of `m:oMath` or a successful fallback PDF export does not prove correct native rendering. When PowerPoint is unavailable, identify that verification limit and provide the accessible preview.

## Write speaker notes as reasoning

- Put only words intended to be spoken in speaker notes. Remove timing blocks, source records, editing comments, delivery or action instructions, and duplicate inventories of slide text. Keep those records in the existing project audit assets; create a separate manuscript only when requested.
- Explain the current visual, its evidence, the design choice or exception, and its conclusion. Connect naturally to the previous idea and the next needed question without repeating a stock transition on every slide.
- Follow the visual reading order, normally left to right and top to bottom. Spoken references such as “The left panel compares…” are useful; bracketed directions such as `[point to the chart]` are not part of the script.
- Cover every substantive item on the page: each figure or panel, method block, equation, key comparison, and conclusion needs an oral explanation. Reuse visible terms and concise labels naturally so the speaker can recover the thread from the page. Coverage does not mean reciting every tick, table cell, reference, or sentence verbatim.
- Do not preview another slide after the final conclusion or at a completed study's endpoint.
- Write complete, natural spoken sentences in the talk's language, with short paragraphs and one idea at a time. Explain displayed equations in words instead of reproducing notation in the script, and define any necessary symbols next to the equation on the slide.
- Keep the speech grounded in the displayed content. Supply the context and technical explanation needed to understand it, but do not introduce an unseen experiment, numerical result, or independent claim. If a result is essential to the spoken argument, give it visible support or revise the slide.
- When the visual already carries exact values, let the audience read them. State the direction, relative size, comparison, and conclusion instead of speaking a sequence of small decimals; read only the few headline values that matter, using sensible rounding when exact precision is not part of the claim.
- For each chart, explain what the axes and visual encodings mean, what is compared and why, the relevant pattern, and its conclusion. With multiple panels, explain each panel's purpose and how the panels jointly support the point. For a method diagram, explain inputs, operations, evidence flow, and outputs; for an abstract analysis, walk through its displayed example. Do not merely read labels or narrate every point.
- Build the explanation from first principles: state what was done, why that choice follows from the problem, and what the evidence means.
- Emphasize the implemented design and observed result. Avoid defensive lists of absent components or repeated `we do not` phrasing unless an exclusion is necessary to define validity, safety, compatibility, or the evidence boundary.
- For bilingual scripts, choose one language as the source of truth, keep language sections in a consistent order, and translate slide by slide so the two versions preserve the same claims, paragraph structure, and emphasis.
- For code-generated decks, keep the slide-aligned script in the generator or in one source file consumed by it, write the script into PPTX speaker notes during the build, and validate note coverage after saving.
- Review slide and speech together in both directions: every meaningful visual must be explained, and every spoken claim must have a clear role in explaining that page. Estimate and, when practical, rehearse the talk duration including pauses for figures; simplify the page map if full coverage will not fit.

## Implement with code

- Use the repository's existing presentation library, helper functions, assets, and template when available.
- Keep reusable code free of personal absolute paths, credentials, and project data. Resolve project assets from the script or repository root.
- Put a multi-project deck and its generator at the shared project level unless the user specifies another location.
- Follow the project's existing runtime and dependency environment. Keep useful assets and audit records in its established structure, and temporary renders or scratch work in temporary storage. Do not add a new top-level work directory or extra deliverables without a task need.
- Use real analysis outputs for charts. Keep source files and metric definitions traceable.
- Apply the font size, weight, contrast, and padding contract above to native objects and generated figures alike.
- Use a PowerPoint slide-number field in the footer when pages are numbered, rather than hard-coded numerals. Covers may omit the field when the design calls for it. Verify numbering after slides are inserted, removed, or reordered.
- Integrate generated figures with the slide palette. For Matplotlib charts placed directly on a page, set the figure, axes, and exported image background to the slide background color. When the chart needs separation, use an intentional same-palette tint or card instead of the library's default white canvas. Keep transparency only when the target renderer has been verified.
- Use the same terminology for a concept in the slide, chart, legend, and notes. Spell out an abbreviation at first use, then use one short form consistently.
- Store speaker notes in the PPTX rather than in a separate file unless the user requests both.
- Generate static slides without animations or transitions unless the user explicitly requests them. Remove inherited effects from copied slides and keep PowerPoint section names and boundaries consistent after reordering or merging slides.

## Validate the delivered file

1. Generate the deck from a clean invocation and reopen the saved PPTX.
2. Run `scripts/validate_pptx.py` for deterministic checks. Treat its geometry and capacity findings as review leads, not rendered truth.
   This validator does not establish font weight, contrast, readability of text inside images, or semantic completeness of notes. Check these in the visual and spoken-content reviews.
3. Render with an installed PowerPoint-compatible application and inspect the actual pages. Check overflow, overlap, line breaks, chart proportions, table density, font substitution or weight changes against the approved baseline, SVG distortion, image borders or background seams inside both figure and axes, page numbers, notes, visible spell-check underlines, and animation residue. Confirm that legends, axes, units, symbols, abbreviations, and comparison groups remain legible at presentation scale. Look specifically for orphaned final lines containing only one word, one or two CJK characters, or another short fragment. Also flag lines that fit in the current renderer but have less than the required `2 em` horizontal reserve. Rewrite or widen the text box before reducing font size, unless the short line is an intentional display treatment.
4. When cross-platform fidelity is required, render with every accessible target application or operating system and compare the resulting pages. A successful render in LibreOffice, Keynote, or a browser viewer does not by itself prove parity with Microsoft PowerPoint. If a required environment is unavailable, name the unverified environment and do not claim full cross-platform validation; provide a PDF preview when it helps the user perform the remaining check.
5. Compare the rendered body with the separator-to-footer content region. Inspect top/bottom and left/right whitespace, the actual plot area after labels and legends, and padding inside raster/SVG assets. A large full-width frame or bottom banner must not hide a small, off-center primary visual. Correct the layout and rerender affected pages. Review information duplication after rendering. Remove repeated takeaway boxes or secondary prose that shrinks the primary evidence without adding a distinct claim.
   Use visual inspection of rendered pages, with a visual-capable model when available. Confirm consistent title geometry, large and strong type, dark readable text, sufficient card padding, and an evidence-led composition. Check final-scale figure labels and strokes; a technically valid SVG or native text box can still be too small or faint. Apply the paired slide-and-speech review to every revised slide.
6. If rendering is unavailable, say so. Do not claim visual inspection from code checks alone.
7. Read back the final output path, slide count, titles, notes coverage, and validation result after any generator or office application changes the file.

For the detailed research-deck workflow and slide-selection rules, read [references/research-ppt-workflow.md](references/research-ppt-workflow.md).

Run the validator with:

```bash
python scripts/validate_pptx.py path/to/deck.pptx --require-notes --min-font 22
```
