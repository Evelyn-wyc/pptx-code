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

## 2. Prepare a page map and evidence ledger

Each page-map row should contain:

- page job;
- topic title;
- takeaway sentence;
- primary visual or table;
- speaking purpose;
- source and comparison basis.

The evidence ledger should record the data source, as-of date, sample, period, benchmark, metric definition, weighting rule, and whether the result is fitted, validated, or replayed. Use it to prevent accidental cross-period comparisons and hindsight leakage.

## 3. Give each slide one task

A slide may introduce the problem, motivate a method, define a rule, show a result, explain a result, or state a boundary. Split the page when these jobs require separate evidence or separate conclusions.

During production, answer this internal prompt:

> What should the audience remember after this slide?

The title, takeaway, visual, and notes should all support that answer.

## 4. Use titles and subtitles deliberately

- Title: a short topic phrase such as `单因子检验`, `组合构建`, or `经营模式分布`.
- Takeaway: the conclusion, such as `综合分决定入选，流通市值决定权重`.

Avoid generic labels that leave the audience guessing about the page's finding. A cover, agenda, section opener, or transition does not need a forced conclusion subtitle.

## 5. Divide work between slide and notes

The slide holds the rule, main number, result, visual evidence, and one-sentence conclusion. Notes carry the reason for the design, calculation details, interpretation of exceptions, limitations, and transition.

A useful speaking sequence is:

1. point to the visual;
2. identify the evidence;
3. explain the design choice or exception;
4. state the conclusion;
5. connect to the next question when one remains.

## 6. Match the visual to the evidence

- Time path: line or area chart.
- Method or group comparison: bar, dot, slope, or compact table.
- Distribution: histogram, box plot, violin plot, or percentile bands.
- Composition: stacked bar, matrix, or a restrained share chart.
- Decision sequence: flow or funnel.
- Exact multi-metric comparison: table.
- Source-backed cases: table with date, original evidence, and rule.
- Up to three short judgments: text cards.

Use the smallest visual that proves the takeaway. A chart should encode data, not decorate a page.

### Make the evidence visual-first

On an evidence slide, choose the primary visual before writing body copy. If a result can be plotted or shown, make that chart, image, matrix, diagram, or compact table the main object on the page. Keep only the takeaway, essential labels, and source visible; move causal explanation, method detail, exceptions, and transitions into speaker notes.

Use SVG with brief text when the evidence is conceptual and no suitable data chart or raster image exists. Do not add decorative images that compete with or imply evidence.

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

Every important judgment should support questions about source, calculation, date, reproducibility, and classification rule. Prefer primary or authoritative sources for policy, industry, and company facts. Preserve the original text, date, and decision basis for qualitative classifications.

## 9. Explain methods at the level needed for the conclusion

Cover the choice, purpose, rule, failure mode, and economic or operational meaning. Keep implementation formats and incidental code details in notes or backup material. A transparent rule, a tree, and an additive or interaction model may share a section when the page makes their different roles explicit.

## 10. State boundaries as research findings

Mixed evidence can still support a decision. Say whether an input is suitable for selection, classification, explanation, monitoring, or no current use. Preserve uncertainty, sample limits, and concentration of returns. Do not turn observation into proof.

## 11. Control information density

Use three visual levels:

1. takeaway for a five-second read;
2. evidence for the main inspection;
3. source and qualification for verification.

Keep ordinary body text at a readable size. If a table needs silent reading time, let the notes first state the overall pattern, then discuss one or two representative entries.

## 12. Allocate time by novelty

Move quickly through background, agenda, and standard procedures. Spend more time on the original method, decisive evidence, surprising result, and boundary. For a 12-minute research talk, a workable starting allocation is 1.5 minutes for the problem, 3 minutes for standard methods, 4 minutes for the central contribution, 2.5 minutes for results and interpretation, and 1 minute for the conclusion. Adapt this to the actual page map.

## 13. Inspect the rendered deck

Use the exported or projected pages as the final visual authority. Check font size, replacement fonts, line breaks, alignment, table crowding, chart aspect ratio, SVG rendering, image borders and background seams, page numbering, notes, and animations. Preserve a manually approved version as the visual reference for later revisions.

## Single-slide test

Use this compact test during review:

> one question + one takeaway + one piece of evidence + one explanation + one transition

Ask whether the slide answers a clear question, states its conclusion, proves it with the right evidence, explains the choice in notes, and connects naturally to the remaining argument.
