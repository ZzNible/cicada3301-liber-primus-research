# K=86 transition signal — selected experiment chain

## Why this matters

In the canonical unresolved LP2 corpus, the strongest local ciphertext-side observation is the unusually low number of adjacent identical runes.

Canonical corpus used by this project:

- GP runes: **12,956**
- valid source-aware adjacent transitions: **12,954**
- observed immediate self-repeats: **86**
- canonical JSON SHA-256: `75772c127e85f73fa5b9838abdad2e6bcf80b352dd9b477d404d5cd29eb4a264`
- raw rune-stream SHA-256: `79b14e630946b64cdca838f328e73904f506df576d15e21fcb46271d4b4c8040`

**Status: SIGNAL. Mechanism: OPEN.**

The important contribution is not just the observation. It is the sequence of dependency repairs and failed explanations that followed.

## What survived

A source-aware exact-count permutation audit leaves the repeat deficit extremely large. In the layout-boundary audit, the baseline statistic was about `Z=-17.43`; after removing every adjacency crossing a frozen non-rune lossless event, the remaining topology still scored about `Z=-15.25`.

This rejects the simple explanation that punctuation/newline/layout flattening manufactured most of the anomaly.

## What initially looked like extra evidence — but was not independent

Two visually striking properties were observed:

1. every diagonal transition cell was a row minimum in the 29x29 transition table;
2. self-transition ranks remained low across broad temporal folds.

Those effects are descriptive facts, but fixed-`K=86` replays showed that they occur naturally once the low repeat count is conditioned on.

### EXP-475 — fixed-K minimum-trace replay

- fixed `K=86` null replays: 20,000
- observed all-29 diagonal-minimum event under the fixed-K null: 15,191 / 20,000
- `p = 0.759562`

**REJECTED scoped:** the all-minima pattern provides substantial evidence independent of K.

### EXP-476 — fixed-K temporal-floor replay

- fixed `K=86` null replays: 20,000
- observed temporal statistic: compatible with the conditioned null
- `p = 0.364982`

**REJECTED scoped:** temporal persistence provides substantial evidence independent of K.

This is a useful warning about double-counting dependent anomalies.

## Other tested explanations

### Layout and representation

EXP-449 removed all transitions crossing frozen punctuation/layout events. The repeat deficit remained extreme (`Z≈-15.25`).

**REJECTED scoped:** flattened punctuation/layout adjacency substantially explains K=86.

Newline/page resets and rubricated-region explanations were also rejected in their tested forms.

### Lag-2 recurrence

EXP-469 tested whether an additional lag-2 anti-recurrence survived after the first-order structure was accounted for.

- observed lag-2 count: 441
- null mean: 456.132
- lower-tail `p = 0.245479`

**REJECTED scoped:** extra lag-2 suppression.

### Solved-LP comparator replication

EXP-470 tested relevant solved comparator streams. Joint calibration did not reproduce the effect (`p≈0.149`).

**REJECTED scoped:** the same self-transition floor is a generic solved-LP property.

### Pure no-repeat code

A Goldman-style q29 no-repeat generator is reversible but necessarily gives `K=0`.

**REJECTED scoped:** pure no-repeat generation explains the observed corpus.

### Maximum run length 2

Under the tested q29 maximum-run-2 generator with the canonical component lengths, expected immediate repeats were about 418 rather than 86.

- mean `K≈418.33`
- SD `≈19.46`
- `P(K<=86)≈4.04×10^-93`

**REJECTED scoped:** this classical hard constraint naturally produces the observed level.

### Soft anti-repeat fit

An external implementation using a soft self-repeat penalty was audited. Its `p_keep` parameter was fitted from the observed repeat rate; the apparent off-diagonal agreement was largely a normalization consequence.

**REJECTED claim:** the fitted parameter independently identifies the mechanism.

A symmetric soft anti-repeat family remains **OPEN as compatibility only**.

## Fixed-K capacity observation

An exact enumerative fixed-K q29 construction exists. Conditioning on exactly 86 repeat locations imposes a codebook deficit of about:

- **327.922 bits**
- equivalent to roughly **67.50 q29 symbols**

This is an **ESTABLISHED mathematical construction**, not evidence that Cicada used it.

## What EXP-477 did not settle

A source-allocation residual test gave an ordinary statistic, but its positive-control power was insufficient for closure.

Therefore:

**OPEN:** some residual state dependence may exist.

Do not cite EXP-477 as proving state-blind generation.

## Current interpretation

The defensible statement is narrow:

> LP2 contains far fewer immediate identical-rune transitions than expected under the tested exact-count permutation baseline, and several simple representation, reset, lag, hard-code and fitted-soft-code explanations have failed.

It is **not** defensible to say:

- we know the encoder is anti-homopolymer;
- we know a particular feedback/autokey mechanism;
- all diagonal minima are a second independent clue;
- the temporal pattern is a third independent clue;
- K=86 itself gives a key or plaintext.

## Reopening criterion

Do not fit another stateful/anti-repeat family merely because it can reproduce 86. A meaningful reopening should provide, before LP2 inspection:

1. an independently grounded operational mechanism; and
2. a new observable/prediction not constructed from K=86.
