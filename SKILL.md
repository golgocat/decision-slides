---
name: decision-slides
description: Create or review restrained business presentations in HTML, PPTX, or Google Slides. Use for bilingual decision decks, option comparison matrices, pilot or scope presentations, executive briefings, and any slide work that needs one message per slide, a decision section separated from a complete appendix record, meaningful structure, intentional line breaks, exclusive Japanese-English switching, and keyboard navigation.
---

# Decision Slides

Create restrained, reader-first presentations that a businessperson can understand on first viewing.

## Establish the message

- Identify the audience, the decision or outcome, and the single narrative before designing slides.
- Give every slide exactly one message. Write that message as a takeaway title, not a topic label.
- Keep only the evidence needed to understand or trust that message.
- Split a slide when two claims compete for attention.

## Separate the decision from the record

- Identify every audience before choosing a structure. A decision deck usually has two: the person who decides, and the person who later verifies or implements. They need opposite amounts of detail.
- Do not interleave them. Put the decision narrative in a main section and the complete record in an appendix in the same document.
- Number the two sections separately, for example `01 / 22` in the main section and `A01 / A23` in the appendix. The reader must always know whether they are reading the argument or looking something up.
- Let the length of the main section be visible and honest. A reader who knows the argument is 22 slides reads differently from one facing 45.
- Moving something out of the main section is not deleting it. Relocate detail to the appendix instead of removing it. Traceability the main section no longer shows must still exist somewhere in the same document; "simplify" must never quietly destroy the audit trail.
- Compress a run of sibling detail slides into one overview table plus the full slides in the appendix. Write each overview row as what the item means for the reader or the build, never as a bare heading. "Guest register and passport" is a table of contents; "Register the people who actually stay, keep it three years, take a passport only where required" is a decision.
- Prefer an appendix over a second document. One file keeps the record attached to the argument through email, print, and archiving.

## Use meaningful structure only

- Add structure only when it communicates grouping, sequence, comparison, hierarchy, causality, ownership, or evidence.
- Do not add decorative metric strips, card grids, repeated boxes, empty numbering, or duplicate summaries.
- Keep catalog versions, internal process labels, and provenance out of the main message unless the audience needs them to decide. Keep supporting source context in the research record or an appropriate appendix, subject to the requested scope; do not add it to the footer by default.
- Prefer open space and one strong composition over dashboard-like density.


## Option comparison matrices

Use this pattern when the reader must choose among a small set of options (typically two to four) on rights, price, ownership, or scope. The comparison itself is the message.

- Prefer one dense comparison slide over a run of per-option slides when the audience needs a pick, not a tour. Keep the full audit trail in the appendix or the research record if needed.
- Order columns by the reader's story, not by source numbering or chronology. A useful default arc is original proposal → derivative / add-on → unconfirmed alternative. Renumber headers to match that order; do not preserve an upstream ①②③ when it fights the narrative.
- Keep only decision-changing axes: fee / SoW, add-ons, existing technology stance, IP ownership, internal use, third-party supply, supply-cut resilience, and a short Notes row. Drop process, history, and status chrome.
- Put jargon definitions on the axis label as a demoted gloss (smaller type under the term), not on a separate glossary slide. Shrink the gloss before shrinking body cells.
- Split compound prices across rows when the table has the rows. Base SoW on one row; OEM or licence add-ons on another. Show total and formula together in the add-on cell when both matter, for example `USD 20,000 (10,000×2)` plus any discount rule that belongs in that cell.
- Keep uncertainty and provenance inside the cell or Notes row for that option. Do not add footer caveats or a second caution strip under the matrix.

## Keep footers minimal

- By default, keep the footer to a page number and, only when useful, a short date or document label.
- Do not add sources, evidence, provenance, caveats, warnings, assumptions, or implementation-status notes to the footer unless the user explicitly requests their inclusion. A general request for research, accuracy, or a proposal is not such a request.
- Apply this default to every slide and language. When revising an existing slide, remove unsolicited footer notes rather than preserving them merely because a template includes them.
- Keep an essential qualification next to the relevant claim in the body or diagram, or rewrite the claim to be accurate. For example, label a planned feature as a proposal in its own block. A simple footer must not turn an unverified or proposed result into a confirmed fact.
- Preserve supporting evidence in the existing research record, speaker notes, or an appendix when the requested format permits it. Do not add slides or footnote-like text along the bottom just to bypass a one-slide limit or the user's request for a simple footer.

## Avoid unsolicited notes and asides

- By default, do not add cautionary notes, supplementary asides, process reminders, or footnote-like disclaimers on slides (注意書き・補足書き). Examples to omit unless the user explicitly asks: "do not send yet", "needs re-approval", "for reference only", "assumption:", or similar status reminders.
- A request to keep the deck accurate or simple is not a request to add those notes.
- If a claim is uncertain, rewrite the claim itself so the uncertainty is in the wording of that cell or sentence. Do not add a separate caution line under the slide or under the table. In an option matrix, put status such as "unconfirmed with the counterparty" or "original / derivative / unconfirmed" in the relevant Notes cell, not under the table.
- Stakeholders, contact rules, and workflow reminders belong in chat, the issue tracker, or the appendix record when needed, not as slide chrome.

## Write for a first-time reader

- Apply a five-second test: a businessperson seeing the slide for the first time should understand its point without narration.
- Apply that test to every slide in isolation. Do not assume the reader saw the previous slide or knows the project vocabulary.
- Use plain language, active voice, and concrete outcomes. Remove internal planning language and implementation trivia.
- Make the title and primary sentence sufficient to understand the slide; supporting details should only clarify or prove them.
- Make every noun, label, and number understandable from the slide itself.
- Keep internal taxonomy and workflow terms out of the main section entirely: `catalog`, `Include`, `Defer`, `REQ-*`, scope versions, and confidence labels such as `P50` or `P80`. When one is essential to the decision, replace it with plain language — `P80` becomes "the planning figure we expect to stay within in roughly eight cases out of ten".
- Use exact identifiers freely in the appendix, and require them there. The appendix is the one place in the document where precision outranks readability; a record that renames its own identifiers is not a record.
- A count is not a message or evidence by itself. Remove unexplained totals, or replace them with the business outcome they are meant to communicate.
- Show a metric only when it answers a reader's business question and includes the necessary unit, denominator, comparison, and decision context.
- Shorten or recompose copy before reducing type size. Split a long reference table across slides before shrinking it: more slides that can be read beat one slide that cannot. Exception: a one-slide option comparison matrix (see Option comparison matrices) may stay dense on a single slide when the decision itself is the comparison.
- Chunk a split table evenly. Use `slides = ceil(rows / max_rows)`, then `rows_per_slide = ceil(rows / slides)`. Slicing by a fixed size instead leaves an orphan final slide holding one or two rows. Around ten rows per slide is a workable maximum for a dense reference table.
- Hold a floor on effective printed size: roughly 8 pt for a dense appendix table, roughly 10 pt for anything in the main section. At a 1280 px print width, `calc(var(--sw) * 0.0086)` renders about 11 px, about 8.3 pt. Compute the printed size from the ratio; do not judge it from a browser window.

## Control line breaks

Line breaks are a property of the composition, not of the copy. Authoring a good break and then letting the layout resize underneath it produces a deck that reads correctly in the PDF and badly on the reader's screen.

- Choose title and lead-sentence line breaks deliberately in each language.
- Keep proper nouns, katakana compounds, numbers with units, and short semantic phrases together.
- Avoid single-word orphan lines and accidental breaks that change emphasis.
- Render Japanese and English separately; a good break in one language is not automatically good in the other.

### Size type from the slide box, never from the viewport

- Define the slide's real width once as a custom property and derive every font size from it: `--sw: min(96vw, 177.78vh)`, then `font-size: calc(var(--sw) * 0.035)`. The slide box and the type then scale together, and composition becomes a property of the deck rather than of the window.
- Do not size type in `vw` while the slide box is height-bound. A wide, short window shrinks the box but not the type, so authored breaks blow out. Print at 1280 × 720 coincidentally agrees with `vw`, which is why PDF-only QA never sees it.
- Do not wrap box-relative sizes in `clamp()`. At large or small boxes the min or max term binds, type stops tracking the box, and the composition drifts again — a clamp is a promise to break proportionality at exactly the sizes you did not test. Hold the floor by choosing the ratio, not by capping it.
- Express slide padding in the same variable. A percentage padding resolves against the containing block, not the element, so `padding: 2.5% 3.2%` tracks the viewport while the type tracks the box, and the text measure silently disagrees with both.
- Draw slide edges with `outline: 1px solid …; outline-offset: -1px`, not `border`. A border participates in layout, so a screen border that print drops changes the measure by 2 px and shifts every printed page. An outline costs nothing.

### Let the browser even the ragged edge

- `text-wrap: balance` on titles and lead paragraphs. It evens a two- or three-line block and removes most orphan last lines without rewriting the sentence. It survives real paginated PDF export — verify this rather than assuming it.
- `text-wrap: pretty` on body paragraphs and list items, where balancing a long block is wrong but a stranded last word is still ugly.
- `word-break: auto-phrase` on Japanese prose. It breaks at phrase boundaries, so 「無人ホテル運営」 no longer splits as 「無人ホテ / ル運営」.
- Never apply `word-break: auto-phrase` to tables. It changes each cell's min-content width and therefore the column widths.
- Reach for these before rewriting copy. Nine orphaned lines are a styling defect, not nine bad sentences.

### Make the line breaks a build contract

- Measure rendered lines, not markup. Walk every text node character by character with a `Range`, group `getBoundingClientRect().top` within a few pixels, and you have the real visual lines and their widths. Authored `<br>` tells you what was intended, never what Chrome did.
- Assert that screen composition equals print composition. Measure each display block at the print size and at a spread of real window shapes — wide and short, narrow and tall — and fail the build when the line count differs. A break that only appears in the browser is a defect the reader sees and the PDF hides.
- Assert no orphan final line: fail when a multi-line block's last line is under about 30 % of its widest line.
- Only `.slide.active` is displayed on screen. Add `.active` to every slide before measuring, or the contract silently checks one slide.
- Key measurements by slide plus an ordinal, not by class name. Two blocks with the same class on one slide otherwise collide and report as a phantom failure.

## Apply the visual grammar

- Use a warm paper canvas, near-black ink, restrained muted text, and fine rules: `#f7f6f2`, `#fbfaf6`, `#11110f`, and `#45433d` are suitable defaults.
- Use a high-contrast serif for display text and a neutral sans serif for labels, metadata, tables, and controls.
- Favor flat editorial compositions. Avoid gradients, shadows, glossy effects, rounded-card dashboards, and ornamental icons.
- Use hairlines only when they express hierarchy, separation, or evidence.
- Make the title slide especially minimal: identity, one proposition, and only essential context.

## Make bilingual decks effortless

- Follow the requested default language; when unspecified for an international business deck, default to English.
- Place a small `日本語 / English` switch at the top right of every slide.
- Prefer exclusive language display: show Japanese or English, never both stacked in the same cell or block. Dense comparison tables become readable only when one language is visible at a time.
- Keep semantic parity between languages while allowing natural rewriting and independent line breaks.
- Preserve the selected language during navigation and reload.
- Keep invariant names, identifiers, and proper nouns consistent across languages.

## Support slide navigation

- Support `ArrowLeft`, `ArrowRight`, `ArrowUp`, `ArrowDown`, `PageUp`, `PageDown`, `Space`, `Home`, and `End`.
- Preserve hash or deep-link navigation when the format supports it.
- Keep focus visible and do not hijack navigation keys while the reader is typing in a form field.
- Add click, touch, print, and mobile behavior only when they serve the delivery context.

## Enforce the design with a build contract

Required when the deck is generated by code. PPTX and Google Slides decks rely on the manual verification list below instead.

- Ship the checks with the deck. A convention that lives only in prose erodes; a convention that fails the build does not.
- Never hand-edit generated output. The next build discards the edit silently. Fix the generator.
- Assert the structure: total slides, main-section count, appendix count, both page-number series, and the presence of every record the appendix claims to hold.
- Scan the main section — not the whole document — for forbidden vocabulary, and fail the build on a match. Report the surrounding text, roughly 90 characters either side. A failure that does not say where it is cannot be acted on.
- Write negative assertions. Assert that the title slide carries no metric strip, no price, and no counts. Decks decay by accretion, and only an assertion of absence resists it.
- Unless explicitly requested, assert that footers contain no source, evidence, or cautionary text; allow only the minimal page/date/document labels.
- When the structure legitimately changes, rewrite the assertions to the new shape. Never loosen or delete an assertion to make a build pass: the counts are the design, not an obstacle to it.
- Expect structural constants in more than one file. A slide count is typically hardcoded in both the validator and the PDF exporter; changing one and not the other fails late.

## Export layout-stable PDFs

- Treat PDF as a separate delivery surface. A correct browser preview is not proof of a correct PDF.
- Export each language as a separate PDF. Do not rely on interactive language controls inside a static document.
- Fix the print page to 16:9 and make every slide exactly one page. Do not inherit an unspecified A4 or Letter page size.
- Hide language controls and other interactive chrome in print while preserving the message, section label, and page number.
- Use print backgrounds and embedded or reliably available fonts so rules, hierarchy, and Japanese glyphs survive export.
- Prevent responsive and screen-viewport rules from changing the print composition. Print dimensions must be explicit and independent from the browser window.
- Scope every responsive rule to `screen`: write `@media screen and (max-aspect-ratio: 4/3)`, never a bare `@media (max-aspect-ratio: 4/3)`. Chrome still evaluates an unqualified viewport query against the live viewport while producing paged output, so a mobile block leaks into the PDF and resizes the printed page.
- That leak does not reproduce under `emulateMedia({media: "print"})`, so no browser-side check will find it. Assert it in the source instead: every `@media` condition must be exactly `print` or begin with `screen and`.
- Compare the real exported PDF against the previous one page by page, not only the new pages. Extract text with coordinates — a word's bounding box tells you the true rendered size, so a 1.54× wider `REQ-004` is a font-size regression you can measure instead of squint at.
- Apply the complete print layout to every slide, including slides hidden on screen. In particular, set the print `display` and `flex-direction` together so inactive slides cannot fall back to a horizontal flex row.
- Prevent print fragmentation and reflow: keep each slide `break-inside: avoid`, keep bounded table containers clipped, and do not let print-only overflow rules move headers, footers, or dense tables outside the page.
- Apply `white-space: nowrap` to `th` as well as `td` when a column must not wrap. A two-character Japanese header such as `法定` otherwise breaks between its characters in a narrow column and renders vertically.
- Validate the final PDF's file signature, page count, page dimensions, and page order.
- Render every final PDF page to an image. Inspect complete contact sheets and representative pages at full size for clipping, reflow, blank pages, broken glyphs, and unintended language mixing.

## Verify before delivery

1. Render every slide in both languages at the intended presentation size.
2. Confirm zero unintended wrapping, clipping, overflow, tiny type, or hidden content.
3. Test language switching, persistence, keyboard navigation, reload, and direct slide links.
4. Read every slide without its neighbors. Apply the five-second reader test and remove anything that needs spoken context.
5. Reconcile every factual claim against the project's binding constraints. A sentence can pass the reader test and still be false: "verify every guest in person" reads well and contradicts an unattended-operation model.
6. Check each language separately for factual drift, not only for tone. Parallel copy can be correct in one language and wrong in the other.
7. Remove at least one decorative or redundant element during the final edit.
8. Do not deliver while any slide contains two competing messages.
9. Do not deliver while a first-time reader can reasonably ask what a visible number, abbreviation, or internal label means.
10. When PDF is requested, verify the PDF itself in every delivered language; never substitute HTML-only QA.
11. Confirm that footer sources and notes appear only when explicitly requested, and that necessary qualifications remain clear in the relevant body content.
12. For an option matrix: columns follow a reader story (and renumbered headers), language display is exclusive, axis glosses are demoted, compound fees are split across the right rows, and uncertainty lives in cells or Notes rather than under the table.
