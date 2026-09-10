# Package-boundary physical representation signals

**Public synthesis through private-lab EXP-505 (2026-09-10).**

No unknown plaintext is established here. This note documents changes and candidate changes in the **physical/document representation** of Liber Primus material, not a key, opcode, cipher reset, or decoding rule.

## Result in one sentence

Two independently measured physical representation phenomena converge cleanly on the preserved material boundary between sequential pages 16 and 17; a third feature, double-quote morphology/frequency, is physically real and fully reconciled on Onion7 but remains incomplete on pre-Onion7 because source-position localization is unresolved for 11 events.

**Overall status: SIGNAL strong for package-dependent representation; mechanism and cryptographic meaning OPEN.**

## 1. The material boundary

A source-custody comparison established that sequential pages `17..74` are byte-identical, under the fixed +17 mapping, to the preserved 58-page Onion7 image package `0..57`, while sequential pages `00..16` are disjoint from that package.

This makes the sequential `16 -> 17` transition a real preserved-object/package boundary rather than a convenient renumbering boundary.

**Status: ESTABLISHED scoped.**

## 2. Red terminal glyph regime

A separate audit of GP-bearing red spans found a sharp terminal-glyph regime change:

- before the material boundary: `15/15` eligible red GP spans terminate with `⁜`;
- after the boundary: `16/16` eligible red GP spans terminate with `⁕`.

The best cut is exactly after sequential page 16.

This observation was retrospective, so it is not presented as a prospective discovery p-value. It is nevertheless physically/documentarily aligned with the independently established package boundary.

A tempting interpretation was also falsified: `⁕` does **not** simply mean “unsolved ciphertext”, because solved terminal pages also use it.

**Status: SIGNAL strong / retrospective; simple solved-vs-unsolved interpretation REJECTED.**

## 3. Isolated vertical two-dot punctuation

A later line began from a preregistered transcription-level observation: Rain notation contains 30 literal `:` events before Onion7 and zero across the 58 Onion7 pages.

This was not accepted at face value. The source images were audited directly.

### Physical calibration

After an explicitly recorded localization correction, the deterministic first-colon sample on pre-Onion7 pages `03,04,06,07,08,09,10,14,15` is:

- `9/9` physical isolated vertical two-dot targets;
- `9/9` matched word-dot controls are physical single dots.

The previous page06 “four-dot exception” was traced to inspection of a nearby separator and was retained in history as a correction rather than silently overwritten.

### Detector development and stop rules

Several intermediate detector attempts were deliberately rejected before using Onion7:

- a raw vertical-pair detector produced 67 false candidates because larger multi-dot marks contain vertical sub-pairs;
- an isolation rule fixed that specificity problem and reproduced all 30 pre-Onion7 colon events exactly page by page;
- one synthetic-negative gate was contaminated by a nearby true target, so that experiment was rejected for protocol validity and no Onion7 result was claimed.

### Frozen out-of-sample Onion7 scan

A fresh experiment then treated all pre-Onion7 material as construction/calibration data. Before fetching/scanning Onion7, the frozen detector passed an anchor-local synthetic gate:

- positives: `72/72`;
- negatives: `0/72`.

It was then run once across all 58 pinned Onion7 JPEGs:

- expected image dimensions: `58/58`;
- automated isolated-two-dot candidates: `0`;
- pages with candidates: `0/58`.

The preregistered exact-zero prediction passed.

**ESTABLISHED scoped:** this frozen detector returns zero isolated-two-dot hits on the 58 preserved Onion7 images.

**SIGNAL strong / convergent:** the physical class that reproduces the pre-Onion7 colon morphology disappears at the material package boundary under a frozen out-of-sample test.

## 4. Double quotes: physical identity established, full package count still open

EXP-493 had independently preregistered `quote_count` as a feature-level representation signal: Rain contains `30` literal double-quote characters on the transcribed pre-Onion7 pages and `14` on Onion7.

That difference was not treated as physical evidence until the source images were checked.

### EXP-502 — deterministic physical identity sample

The first Rain quote on each of the 13 quote-bearing pages was frozen before image adjudication, with matched word-dot controls.

A first generic line localizer failed on 5/13 pages and was **not** retuned. A fallback then reused image geometry from an older independent exhaustive rune audit rather than parameters learned from quote outcomes.

Result:

- quote-like paired-stroke targets: `12/13`;
- matched physical single-dot controls: `12/13`;
- quote-like controls: `0`;
- pre-Onion7 guard: `5/6`;
- Onion7 guard: `7/7`;
- page08 retained as an explicit alignment failure.

The recurring quote glyph is physically distinct from the small word dot: two narrow approximately vertical strokes rather than a small square dot.

**ESTABLISHED scoped:** Rain literal `"` tracks a genuine visible quote-like physical class on the deterministic cross-package sample.

### EXP-503 — invalid unit of analysis caught by controls

A first full-event reconciliation classified an entire inter-rune punctuation interval as quote-like whenever it contained the quote pair. That made matched word-dot controls on pages24 and60 false positives because a quote and a word dot occupy the same physical interval.

The preregistered negative-control gate failed and the full 44-event score was never run.

**REJECTED scoped:** interval-level quote/non-quote classification is not a valid event classifier.

### EXP-504 — multiplicity-aware event grouping

The next experiment grouped Rain quote tokens by inter-rune interval and compared their multiplicity with non-overlapping physical quote pairs.

Controls passed:

- `12/12` localized quote anchors contained a physical pair;
- `0/10` eligible distinct-interval word-dot controls contained a quote pair;
- the two previously known shared-interval controls were prospectively excluded from the negative set.

Full frozen-manifest result:

- Rain quote events: `44` in `39` grouped intervals;
- localized quote events: `33/44`;
- exact multiplicity groups: `28/29` localized groups;
- reconciled localized events: `32/33`;
- Onion7: **14/14 Rain quote events physically reconciled as 14 quote pairs**;
- 11 pre-Onion7 events remain unlocalized under the inherited exact-count geometry;
- one localized page08 interval contains two Rain quote tokens but only one counted physical quote pair.

Because localization coverage was only `75%`, the registered full-reconciliation criterion failed.

**ESTABLISHED scoped:** all 14 Onion7 Rain quote events are physically reconciled by this frozen method.

**SIGNAL:** quote transcription is highly faithful among localized intervals.

**OPEN / INCONCLUSIVE:** full physical `30 vs 14` package counts.

### EXP-505 — do not rescue the 11 failures by tuning a locator

A separate source-context locator was preregistered for the 11 unresolved pre-Onion7 events. Before those targets could be scored, it had to reproduce at least 90% of already-resolved positive groups and produce zero false positives on eligible word-dot controls.

It failed both conditions narrowly:

- exact positive groups: `25/28 = 0.892857`;
- negative false positives: `1/10`.

The stop rule fired. **The 11 target events were not scored.**

**REJECTED — protocol feasibility / NO TARGET RESULT.** Further crop/localizer tuning is on hold unless an independently motivated source-position method appears.

## 5. What this changes

The useful conclusion is **not** that punctuation is a secret code.

The stronger and more conservative conclusion is that the preserved material packages have real, measurable representation differences, and source-image validation is important because normalized transcriptions lose or conflate physical distinctions.

The quote branch also shows why controls matter: a result can be physically real while a proposed *unit of analysis* is wrong.

This supports treating Liber Primus as a document with potentially typed representation layers rather than assuming every visible convention is decorative or that every page belongs to one homogeneous representation regime.

## 6. What this does not license

These results do not establish:

- a cipher/key reset at page 17;
- an opcode or ASCII interpretation of punctuation;
- a cause for the `K=86` ciphertext anomaly;
- plaintext;
- a binary punctuation channel;
- numeric semantics for community delimiter labels;
- a causal claim that package membership itself determines quote frequency.

Any cryptographic use of the package boundary still needs an **independent ciphertext prediction** fixed before testing.

## 7. Reusable methodological lesson

The most useful part for other researchers may be the protocol history:

1. freeze the transcription-level candidate;
2. verify its physical identity against pinned images;
3. use matched punctuation controls;
4. record localization mistakes explicitly;
5. reject detector versions that fail held-out specificity or synthetic gates;
6. keep target data unscored when the registered gate fails;
7. distinguish a physical glyph from the logical event it represents;
8. do not convert a representation result into crypto semantics without a new prediction.

This sequence prevented several plausible-looking but invalid conclusions from being promoted.

## Current next question

Rather than iterating more quote-localization heuristics, the private lab is moving to an independent question: **does the pre-Onion7 / Onion7 material split extend to the rendering geometry of ordinary black GP runes when punctuation and rubrication are excluded?**

That test can distinguish a broad production/template/rendering-regime change from discontinuities confined to selected annotation classes.
