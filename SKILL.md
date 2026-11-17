---
name: pptx-code
description: Plan, generate, revise, and validate code-driven PowerPoint decks when narrative, evidence, charts, speaker notes, or layout fidelity matter. Use for .pptx creation or editing; skip when the user only wants a prose outline.
---

# PPTX Code

Help the audience follow the research, inspect its evidence, and understand the conclusion without reading dense prose.

These are this user's defaults. The current brief takes precedence; preserve approved content outside the requested scope. Keep project palettes, fonts, filenames, runtimes, and page counts in the project.

## Plan before coding

- Establish audience, time limit, research question or decision, evidence, and visual baseline. For revisions, inspect the latest saved user-approved or manually adjusted deck; preserve unrelated edits, respect output naming, and update its generator.
- Organize completed work as question → reason for the comparison → evidence → interpretation → next question or decision. Follow logical dependencies; distinguish exploration from hypothesis testing and retrospective explanations. Independent studies may establish separate premises.
- Review a page map before construction. Each row records question/job, reason and comparison, short title, internal takeaway, primary visual, speaking purpose, next connection, and source. The author or assisting AI may perform this review within the task's authorization. The takeaway is planning metadata, not a required subtitle.
- Keep an evidence ledger: source, cutoff/as-of date, period, sample/eligibility, metric and weighting definitions, benchmark, and fitted/validation/replay status. Keep paths, notebook cells, timing estimates, build records, and incidental configuration there or in existing audit assets.
- Use compact, standard bibliographic citations with consistent placement; a bare URL or hyperlink is insufficient for a paper. Web references may use descriptive links.
- Allocate pages and speech by novelty, importance, and available time. Define unfamiliar concepts plainly or with one stable introductory analogy, then return to technical terms. Keep secondary metrics, derivations, and implementation detail available for questions. A completed study may end with its conclusion and boundary.

For research argument design, visual selection, and body positioning, read [research-ppt-workflow.md](references/research-ppt-workflow.md).

## Template, typography, and layout

- Use the supplied template or obtain the intended visual direction before authoring; this skill supplies no default template. Inspect masters, layouts, theme, placeholders, footers, and examples. Identify a design by master/layout, not slide number; keep it consistent across generated pages unless an intentional section change requires otherwise.
- Match the approved rendered appearance, including typeface, weight, and density. Resolve substitutions into explicit font choices. Write separate Latin and East Asian font settings into the PPTX where supported; use fonts available on target systems or record an installation/substitution plan. Verify appearance in the target application.
- Ordinary titles share size, weight, and position, normally **30–32 pt bold**. Authored body text and key chart labels normally use **at least 22 pt bold/semibold**; references and secondary captions may use **18 pt**, template footers smaller. Verify visible weight and final-scale text inside images/SVGs too. Enlarge or simplify content before reducing type size.
- Use dark, high-contrast substantive text and equally readable comparisons. Prefer light content backgrounds; use coordinated accents and dark panels only within the approved design.
- Give cards and text boxes visible padding and vertical room for line/paragraph spacing and font substitution. For ordinary CJK or mixed text, reserve **2 em of unused width on each intended line after margins**; use a comparable reserve for other scripts. Use intentional breaks; widen or rewrite before shrinking. AutoFit and zero margins do not provide this reserve.
- Use simple card fills/borders and hierarchy through typography, spacing, and color. **Omit decorative vertical strips on either card edge.**
- **Omit routine bottom explanatory lines, takeaway ribbons, and experimental-configuration fine print near page numbers.** Put explanation in notes and incidental configuration/provenance in the ledger. Keep essential comparison conditions, axes, units, and legends readable with their visual. Retain template page numbers and compact source citations; full references may use a reference slide.
- Center the complete visible body within the template's content region: below the title separator/header and above the footer or necessary source block, within its side margins. Balance actual ink and visual weight, including charts, labels, tables, and copy; ignore unused image padding. Preserve internal alignment and intentional asymmetry. A centered bounding box or full-width decoration cannot compensate for undersized evidence. Follow the reference's [body-region procedure](references/research-ppt-workflow.md#body-region-layout).

## One job per slide

- Use a short, informative topic title. Omit routine summary/conclusion subtitles unless requested, decorative eyebrows, and part-number prefixes; use sections or section openers for navigation. Covers/agendas may retain their approved hierarchy. Prefer concrete conclusions to unexplained abstract labels.
- Let the dominant chart, figure, diagram, or coherent panel set carry the evidence. Keep prose to essential labels and helpful local annotations; explain it in notes. Use three levels: title → evidence → source/qualification. Avoid repeating a finding in title, banner, and card.
- Reuse original paper figures, PPT assets, or HTML image sources before screenshots or reconstruction. Preserve scientific meaning, resolution, aspect ratio, and legible labels; crop/enlarge/rearrange relevant panels when needed. Use native diagrams/SVGs for a conceptual explanation without a suitable source figure.
- Give each visual one analytical purpose. Repeat a chart only when its annotation, comparison basis, or question materially changes. Prefer charts for trends/distributions/comparisons, tables for exact comparable metrics or rules, and a few cards for compact judgments. Merge sparse pages answering one question; split dense pages with competing conclusions. Remove redundant callouts that crowd the main visual.
- Make evidence self-contained: identify axes, units, periods, samples, colors, marks, line styles, and groups; define symbols/abbreviations at first use and explain aggregation, missingness, padding, or transformations. Label incompatible periods/samples separately. For controlled comparisons, show what changes, what stays fixed, and the contrasts needed for the component claim.
- Explain why a method is chosen, what it solves, how it works, and its failure conditions. Describe what the technical contribution changes in the inference. Connect evidence to operational/domain meaning, not just another metric description.
- Match claims to evidence. A point estimate is an observed gain; claims of significance, robustness, or inconclusiveness need uncertainty, repeated-fit, or sensitivity support. Preserve mixed evidence and state the use it supports, its limits, and the remaining uncertainty.
- Covers identify topic, speaker, and affiliation; add result metrics only for a relevant executive-summary use case. Every non-appendix page belongs to the spoken path; add an appendix only for genuinely optional material. Close completed studies with contribution and decisive supported findings, including efficiency/cost when relevant, without filler plots or a forced next step.

## Native equations

- Use editable PowerPoint Office Math (OMML), equivalent to Alt+=, for displayed mathematics. Build structural fractions, indices, powers, sums, roots, and matrices; ordinary text, Unicode approximations, or formula images alone are insufficient.
- Keep prose outside math objects, use a supported math font, define symbols/indices near first use, and explain each expression's purpose and computation in speech.
- Derive native output and any compatibility fallback from one authoritative expression. Package fallback as alternate content, not a second visible formula; verify mathematical equivalence, especially scope, signs, limits, and denominators.
- Check saved OMML and inspect native Microsoft PowerPoint rendering when accessible: structure, legibility, bounds, and inline alignment. OMML presence or a fallback PDF alone cannot establish native correctness. If PowerPoint is unavailable, state that limit and supply the available preview.

## Speaker notes

- Store the slide-aligned script in the PPTX, sourced from the generator or one file it consumes. Create a separate manuscript only if requested.
- Notes contain only natural spoken prose: complete sentences, short paragraphs, one idea at a time. Keep timings, source/build records, editing comments, stage directions, and duplicate slide-text inventories in project records.
- Follow visual reading order. Explain every substantive panel, diagram block/flow, equation, comparison, and conclusion: what the visual encodes, why the comparison matters, what it shows, and its qualification. Spoken references such as “The left panel…” are useful; bracketed delivery instructions are not.
- Explain formulas in words and charts through axes, encodings, patterns, and domain meaning. Cover key labels/findings without reciting every tick or decimal; let visible exact values be read, and speak only the few headline numbers with appropriate precision.
- Ground speech in displayed evidence. Do not add unseen experiments, numbers, or independent claims; give essential claims visible support. Explain the implemented design and observed result directly; include exclusions only when necessary for validity, safety, compatibility, or the evidence boundary.
- Connect ideas naturally without stock transitions. End at the study's conclusion. For bilingual scripts, choose a source language and translate slide by slide with consistent ordering, claims, paragraphs, and emphasis.
- Review slides and speech in both directions: every meaningful visual has an explanation and every spoken claim helps explain that page. Estimate/rehearse duration with pauses for figures; simplify content if coverage will not fit.

## Code and assets

- Reuse repository libraries, helpers, template, assets, and runtime. Use real analysis outputs and traceable metric definitions. Resolve assets relative to script/repository roots; reusable code contains no personal absolute paths, credentials, or project data.
- Put multi-project decks and generators at the shared project level unless directed otherwise. Keep useful assets/audits in the established structure and scratch/renders in temporary storage; avoid unnecessary directories or deliverables.
- Apply typography, contrast, and padding to native and generated objects alike. Match chart figure, axes, and export backgrounds to the slide, or use a deliberate same-palette tinted panel. Verify transparency in the target renderer.
- Keep terminology consistent across slides, figures, legends, and notes; expand abbreviations at first use.
- Use native slide-number fields and verify numbering after reordering/insertion/deletion; covers may omit them. Keep sections synchronized. Default to static slides; remove inherited animations/transitions unless requested.

## Validate delivery

1. Build cleanly and reopen the saved PPTX. Run the bundled validator; geometry/capacity findings are review leads, not rendered truth:
   ```bash
   python scripts/validate_pptx.py path/to/deck.pptx --require-notes --min-font 22
   ```
2. Render and inspect actual pages in the target application, using Microsoft PowerPoint for native-equation checks when available. Check overlap/overflow, orphaned lines, 2 em reserve, title consistency, visible weight/contrast, substitutions, image text/strokes, padding, body balance, chart proportions, table density, SVGs, background seams/borders, numbering, notes, spell-check marks, and inherited effects. Code checks cannot establish these visual properties or semantic note coverage.
3. Review slide and speech together. Remove repetition and ensure the primary visual uses enough area; correct and rerender affected pages. Geometry/pixel bounds support, but do not replace, visual judgment.
4. When cross-platform fidelity is required, compare every accessible target system/application. LibreOffice, Keynote, or browser output does not prove PowerPoint parity. Name unavailable renderers/targets and provide a preview where useful; never claim visual or cross-platform validation from code checks alone.
5. After any generator or office change, read back the final path, slide count, titles, note coverage, and validation results.
