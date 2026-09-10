# Current Research State

**Updated 2026-09-10 through private-lab EXP-505.** No unknown plaintext is established.

## Canonical LP2 corpus

- 12,956 Gematria Primus runes.
- 12,954 valid adjacent transitions under the current source-aware topology.
- 86 immediate self-repeats.
- Canonical JSON SHA-256: `75772c127e85f73fa5b9838abdad2e6bcf80b352dd9b477d404d5cd29eb4a264`.
- Raw rune-stream SHA-256: `79b14e630946b64cdca838f328e73904f506df576d15e21fcb46271d4b4c8040`.

## LP2 transition signal

**SIGNAL / mechanism OPEN:** `K=86` remains the cleanest local ciphertext anomaly.

Secondary descriptions that initially looked independently supportive — including all-diagonal row minima and a temporal self-repeat floor — lose substantial evidential weight once the repeat count is fixed in the null model. These are therefore not three independent clues.

Several simple explanations were tested and rejected within scope, including pure no-repeat coding, a uniform max-run-2 generator, and preserved-source immediate-state/feedback/anti-repeat prescriptions sufficient to reopen arbitrary stateful fitting.

## Physical package / representation boundary

**ESTABLISHED scoped:** sequential pages `17..74` match the preserved Onion7 `0..57` image package exactly under the fixed +17 mapping, while sequential `00..16` are disjoint from that package.

Two representation phenomena converge cleanly on that material boundary:

1. **SIGNAL strong / retrospective:** eligible GP-bearing red spans show `15/15 ⁜` before the boundary and `16/16 ⁕` after it. The simple claim that `⁕` means unresolved ciphertext is rejected because solved terminal pages also use it.
2. **SIGNAL strong / convergent:** a physical isolated vertical two-dot punctuation class calibrated on pre-Onion7 material disappears in a frozen out-of-sample Onion7 scan. The final detector passed `72/72` synthetic positives and `0/72` synthetic negatives before scanning, then returned `0` candidates across all `58/58` pinned Onion7 JPEGs.

A third feature — double quotes — is physically real but not yet fully reconciled across both packages:

- **ESTABLISHED scoped (EXP-502):** Rain literal `"` maps to a genuine paired-stroke quote-like physical class on a deterministic cross-package sample.
- **REJECTED scoped (EXP-503):** classifying a whole punctuation interval as quote/non-quote is invalid because quote and word-dot can share an interval.
- **ESTABLISHED scoped (EXP-504):** all **14/14 Onion7** Rain quote events reconcile physically; among localized groups overall, 28/29 have exact quote multiplicity and 32/33 localized events reconcile.
- **OPEN:** 11 pre-Onion7 quote events remain unlocalized under the inherited exact-count geometry; one localized page08 interval has two Rain quote tokens but one counted physical pair.
- **REJECTED protocol feasibility / NO TARGET RESULT (EXP-505):** a count-tolerant alternative localizer failed its calibration gate before those 11 targets were scored (25/28 exact positives; 1/10 negative false positives).

**No cryptographic semantics follow from these representation results.** The package boundary is not currently evidence of a key reset, cipher switch, opcode, plaintext, or cause of `K=86`.

See `experiments/PACKAGE_BOUNDARY_PHYSICAL_SIGNALS.md` for the detailed public synthesis and failed-protocol guardrails.

## Mixed document architecture

The package result strengthens — without proving — the working model that Liber Primus should be treated as a potentially **typed/mixed document architecture**, not only as one homogeneous rune stream.

Rubrication, physical punctuation/glyph inventory, semantic prime-GP verification, ciphertext transition behavior and the external `AN END` verifier may occupy different functional layers.

**SIGNAL / favored framing; mechanism OPEN.**

The model becomes useful only when a structural feature makes a new frozen prediction. It must not license arbitrary punctuation alphabets, reset fitting, or offset mining.

## Cross-round reuse

**ESTABLISHED scoped:** Cicada deliberately reused representation/semantics across campaigns in at least one documented path:

`Patience is a virtue -> Gematria Primus sum 761 -> 2014 marker 761`.

This proves cross-round composition exists. It does **not** imply that arbitrary prior-round files are valid LP2 keys or pads.

## CicadaOS

**ESTABLISHED historical provenance:** the 2013 CicadaOS path and the historical roles of `_560.00`, `560.13`, and `560.17` are source-grounded.

**REJECTED scoped:** preserved 2014 source material does not independently prescribe those bytes as LP2 input.

## AN END

**ESTABLISHED:** the solved text states that a page in the deep web `HASHES TO` the exact published 512-bit value.

**OPEN:** hash algorithm, exact page/object, serialized bytes, URL/body/file representation, normalization/encoding and historical custody.

The source does not itself say `SHA-512`.

## Public-source ceiling

A bounded audit across additional public repository surfaces recovered zero new qualifying 2012–2014 source objects from the surfaces that resolved and could be inspected.

This is an **OPEN / bounded negative**, not proof that no private/deleted/unresolved artifact survives. Source-recovery outreach should not block experimental work on already preserved objects.

## Current next question

Rather than iterate more quote-localization heuristics, the private lab is testing a genuinely independent document-production explanation:

> Do the pre-Onion7 and Onion7 materials preserve different **ordinary-rune rendering/typesetting fingerprints** even after punctuation and rubrication are excluded and rune identity is controlled?

A positive held-out result would support a broader template/export/render-pipeline regime change. A powered negative would suggest that the observed discontinuities are selective annotation/punctuation phenomena rather than a global rendering change.

## Overall posture

The project remains **evidence-gated rather than compute-gated**. The current shift is deliberate: ask what physical/document object was produced before inventing another cipher family.
