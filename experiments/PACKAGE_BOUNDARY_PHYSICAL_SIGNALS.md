# Package-boundary physical representation signals

**Public synthesis through private-lab EXP-501 (2026-09-10).**

No unknown plaintext is established here. This note documents a change in the **physical/document representation** of Liber Primus material, not a key, opcode, cipher reset, or decoding rule.

## Result in one sentence

Two independently measured physical representation phenomena converge on the same preserved material boundary between sequential pages 16 and 17.

**Status: SIGNAL strong / convergent. Mechanism and cryptographic meaning: OPEN.**

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

## 4. What this changes

The useful conclusion is **not** that `:` is a code.

The stronger and more conservative conclusion is that the pre-Onion7 and Onion7 materials use measurably different physical glyph/punctuation inventories, and two independently studied phenomena converge on the same preserved package boundary.

That supports treating Liber Primus as a document with potentially typed representation layers rather than assuming every visible convention is decorative or that every page belongs to one homogeneous representation regime.

## 5. What this does not license

These results do not establish:

- a cipher/key reset at page 17;
- an opcode or ASCII interpretation of the two-dot mark;
- a cause for the `K=86` ciphertext anomaly;
- plaintext;
- a binary punctuation channel;
- numeric semantics for community delimiter labels.

Any cryptographic use of the package boundary now needs an **independent ciphertext prediction** fixed before testing.

## 6. Reusable methodological lesson

The most useful part for other researchers may be the protocol history:

1. freeze the transcription-level candidate;
2. verify its physical identity against pinned images;
3. use matched punctuation controls;
4. record localization mistakes explicitly;
5. reject detector versions that fail held-out specificity or synthetic gates;
6. keep the target package untouched until the detector is frozen;
7. scan it once;
8. do not convert a representation result into crypto semantics without a new prediction.

This sequence prevented several plausible-looking but invalid conclusions from being promoted.

## Current next question

A third preregistered representation feature — double-quote frequency — is being physically validated separately. It should not be folded into a general punctuation grammar until that independent test is complete.
