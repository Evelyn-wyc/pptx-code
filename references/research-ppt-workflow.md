# Research presentation workflow

Use this reference when a deck must explain a research project, compare methods, defend conclusions, or support an oral presentation.

## 1. Start from audience questions

Write the likely questions before writing slide titles:

1. Why is the problem worth studying?
2. Which gap or constraint matters?
3. What is the research path?
4. Why does each step follow from the previous one?
5. What does the evidence show?
6. Where does the method stop being reliable?
7. What work remains, if the study is still open?

Use these questions as an answer chain. For a completed study, close with the selected method, evidence, and boundary. Add future work only when it is part of the research state or the user asks for it.

### Review the argument before construction

Inventory the completed work, then record each experiment or activity as:

`question / phenomenon → reason for the comparison → evidence and controls → supported interpretation → next question`

The author or assisting AI reviews this map before building slides. A useful test is whether each page can finish the sentence “We examine this because the preceding evidence leaves … unresolved.” An independent result can instead establish a needed premise; the sequence does not have to force every study into one causal chain.

Use the actual status of the work. An exploratory experiment may reveal a pattern, a controlled comparison may test an explanation, and a follow-up may diagnose a failure. Distinguish those roles instead of retroactively claiming every experiment was designed to confirm the final conclusion. Keep mixed and negative evidence when it changes the inference. Put studies in the order the audience needs to understand them, and select visuals only after their argumentative jobs are clear.

## 2. Prepare a page map and evidence ledger

Each page-map row should contain:

- question and page job;
- reason for the experiment at this point and the comparison it uses;
- topic title;
- takeaway sentence for internal planning;
- primary visual or table;
- speaking purpose and connection to the next question;
- source and comparison basis.

The evidence ledger should record the data source, as-of date, sample, period, benchmark, metric definition, weighting rule, and whether the result is fitted, validated, or replayed. Use it to prevent accidental cross-period comparisons and hindsight leakage.

## 3. Give each slide one task

A slide may introduce the problem, motivate a method, define a rule, show a result, explain a result, or state a boundary. Split the page when these jobs require separate evidence or separate conclusions.

During production, answer this internal prompt:

> What should the audience remember after this slide?

The title, visual, and notes should all support that answer. The planning takeaway need not appear as a sentence on the slide.

## 4. Keep titles short and consistent

- Use a short topic phrase that identifies the page's job, such as `Detection Results`, `Event Claims`, or `组合构建`.
- Keep ordinary titles at the same size, weight, and position. Use the font contract in `SKILL.md`.
- Do not add a summary sentence beneath the title unless explicitly requested. Keep the internal takeaway in the page map and spoken explanation; use a local chart annotation only when it clarifies the evidence.
- Omit decorative labels above titles and routine part-number prefixes. Use PowerPoint sections or dedicated section slides for navigation when useful.

Balance brevity with meaning: the title should identify what the audience is about to see. A cover, agenda, or section opener can use its approved hierarchy.

## 5. Divide work between slide and notes

The slide carries the visual evidence, essential labels, and decisive numbers. Notes explain the displayed content in natural spoken language, including the reason for the design, interpretation, necessary qualifications, and transitions. Keep source records, timings, editing comments, action directions, and duplicated slide-text lists in project records rather than speaker notes.

A useful oral sequence, adapted to the actual visual, is:

1. connect the page to the preceding idea;
2. explain what the chart axes and marks, or diagram blocks and arrows, represent;
3. explain the question and comparison in each meaningful panel, in visual order;
4. interpret the result and any qualification needed for that interpretation;
5. connect to the next unresolved question, ending naturally on the conclusion slide.

These are drafting decisions, not stage directions to paste into notes. A phrase such as “The right panel tests whether…” is spoken prose. Every substantive visual should be explained, and every spoken claim should help explain the current page. Cover key labels and findings without reading every number or adding experiments that the audience cannot see.

## 6. Match the visual to the evidence

- Time path: line or area chart.
- Method or group comparison: bar, dot, slope, or compact table.
- Distribution: histogram, box plot, violin plot, or percentile bands.
- Composition: stacked bar, matrix, or a restrained share chart.
- Decision sequence: flow or funnel.
- Exact multi-metric comparison: table.
- Source-backed cases: table with date, original evidence, and rule.
- Up to three short judgments: text cards.

Choose the visual that makes the comparison easiest to understand at presentation scale. A chart should encode data, not decorate a page.

### Make the evidence visual-first

On an evidence slide, choose the primary visual before writing body copy. If a result can be plotted or shown, make that chart, image, matrix, diagram, or compact table the main object on the page. Keep visible text to essential labels, brief annotations, and sources; explain the evidence in speaker notes. Multiple related panels can share a page when they answer one question and remain readable.

Reuse suitable original research figures, PPT assets, or original HTML image files before reconstructing them or capturing rendered pages. Enlarge or crop relevant panels to preserve sharpness and legible labels. Use native diagrams or SVGs for a conceptual explanation that has no suitable source visual. Do not add decorative images that compete with or imply evidence, or replace plots with a sequence of text cards.

### Match generated-image backgrounds to the slide

Treat chart background as part of the slide system rather than an export default.

- For a chart intended to sit directly on the page, use the exact slide background color for the Matplotlib figure, every axis, and `savefig` output.
- When visual separation is useful, choose a restrained tint from the same palette and apply it consistently as a deliberate chart card.
- Avoid an opaque white image rectangle on a non-white slide unless the contrast is intentional and repeated elsewhere in the deck.
- Verify transparent exports in the actual PowerPoint-compatible renderer before relying on them; transparency and SVG handling can differ by application.
- Inspect labels, legends, plot limits, and aspect ratio after placement. A seamless background does not compensate for a chart that is compressed, clipped, or illegible.

## 7. Keep comparisons on one basis

Before placing results together, verify:

- period;
- sample and eligibility rules;
- metric definition;
- benchmark;
- weighting rule;
- information cutoff;
- fitted, validation, or replay status.

Separate incompatible periods or samples. Label them directly rather than relying on a footnote to repair an ambiguous comparison.

## 8. Leave an evidence trail

Every important judgment should support questions about source, calculation, date, reproducibility, and classification rule. Prefer primary or authoritative sources for policy, industry, and company facts. Preserve the original text, date, and decision basis for qualitative classifications in the evidence ledger. Visible paper references use standard bibliographic citations; speaker notes contain the actual talk.

## 9. Explain methods at the level needed for the conclusion

Cover the choice, purpose, rule, failure mode, and economic or operational meaning. Explain implementation details in speech only when they help interpret the displayed method; keep incidental formats and code details in project records or requested backup material. A transparent rule, a tree, and an additive or interaction model may share a section when the page makes their different roles explicit.

Organize related work around the obstacles it leaves unresolved, with a specific and fair limitation for each comparison. Introduce the overall framework before explaining its modules. Explain what each module receives, does, and returns. Use a worked example or diagram to make an abstract analysis understandable before expanding the formal argument. Place retrospective mechanism studies where their role in explaining the observed result is clear.

## 10. State boundaries as research findings

Mixed evidence can still support a decision. Say whether an input is suitable for selection, classification, explanation, monitoring, or no current use. Preserve uncertainty, sample limits, and concentration of returns. Do not turn observation into proof.

## 11. Control information density

Use three visual levels:

1. topic title for orientation;
2. evidence for the main inspection;
3. source and qualification for verification.

Apply the size, weight, contrast, and padding contract in `SKILL.md`, including text inside imported figures and SVGs. If a table needs silent reading time, let the speech first state the overall pattern, then discuss one or two representative entries. Merge sparse neighboring slides that answer the same question; split a dense page when distinct conclusions compete. Preserve generous text-to-frame padding while using enough of the page for substantive evidence.

## 12. Allocate time by novelty

Move quickly through background, agenda, and standard procedures. Spend more time on the original method, decisive evidence, surprising result, and boundary. Allocate time using the page map and estimate or rehearse the spoken script with pauses for figures. When it runs long, reduce secondary content or merge overlapping pages; do not compensate by shrinking type, rushing speech, or leaving displayed evidence unexplained.

## 13. Inspect the rendered deck

Use the exported or projected pages as the final visual authority, with visual-model review when available. Check font size and weight, text contrast, replacement fonts, title consistency, line breaks, padding, alignment, table crowding, chart aspect ratio, SVG rendering, image borders and background seams, page numbering, notes, and inherited effects. Follow the cross-platform checks in `SKILL.md`; native text-box checks cannot assess text embedded in figures. Read the speech beside each revised page to check coverage, natural transitions, and numerical consistency. Preserve the latest manually approved version as the reference for later revisions.

## Single-slide test

Use this compact test during review:

> one clear question + sufficient visual evidence + a supported conclusion + a complete spoken explanation

Ask whether the page answers its question, makes the evidence easy to read, and explains every meaningful visual in natural speech. Connect to the remaining argument when there is one; the conclusion ends the talk. This is a review test, not a set of text boxes to add to the page.


## Body-region layout

1. **Locate the content rectangle.** Read the actual master and slide geometry. The top boundary is the bottom of the title separator plus its intended clearance. If there is no separator, use the bottom of the approved header block plus clearance. The bottom boundary is the top of the footer or fixed source band minus clearance. Use the template's left and right content margins. Title, separator, footer, and page number stay outside this rectangle; it is not the entire slide.
2. **Identify visible content.** Treat the primary chart and its axes, ticks, legend, annotations, table, cards, and body copy as one composition. Include captions and takeaways that are part of the slide's argument. Ignore hidden objects, transparent extents, background-only rectangles, and unused image padding when assessing where the content actually appears. Crop unnecessary asset padding or rebuild the plot before compensating with slide offsets.
3. **Balance the group.** Translate the composition together until upper/lower and left/right unused space are approximately balanced in the content rectangle. Preserve internal reading order, chart-label relationships, column alignment, and left alignment inside text boxes. Centering a group does not mean setting every paragraph to centered text. For intentionally asymmetric layouts, retain the hierarchy and assess visual weight rather than imposing geometric symmetry on every object.
4. **Allocate enough area to the evidence.** An evenly centered but undersized chart is still a poor layout. Enlarge the usable plot region, reduce repeated callouts, or move supporting figures into a compact strip. A wide bottom takeaway can make the bounding box look centered while the primary evidence remains crowded above; review those internal gaps separately. Do not use a decorative frame to satisfy a centering check.
5. **Review rendered pages.** Inspect actual ink and data geometry in a target-application render at presentation scale. Check all four outer gaps, primary-visual size, and internal spacing. Geometry or pixel bounds are diagnostics, not proof of optical balance. Move, resize, or rebuild the content as needed and rerender affected pages; record intentional asymmetry when it materially affects the layout judgment.
