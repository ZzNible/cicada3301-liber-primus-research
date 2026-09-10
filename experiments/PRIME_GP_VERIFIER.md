# Prime-GP plaintext verifier — selected experiment chain

## Main result

A reproducible structural property exists on a source-defined class of solved Liber Primus statements: their Gematria Primus sums are prime.

This is one of the strongest positive findings in the project because it lives on the **plaintext side** and was later given a prospective holdout.

**Status:** `ESTABLISHED structural relation / SIGNAL lightweight verifier role`.

It is **not** a decoder, key, keystream, offset or mapper selector.

## EXP-275 — frozen 17-statement core

The first bounded reproduction used solved content statements under the source-defined roles `WIDSOM`, `SOME WISDOM`, and `AN INSTRUCTION`.

Result:

- **17 / 17** statement-level GP sums were prime.

The sums were:

`1009, 991, 991, 941, 751, 853, 1039, 1237, 773, 1399, 1583, 601, 643, 727, 971, 383, 571`

Useful negative controls around the same material include composite headings:

- `WIDSOM` -> 270
- `SOME WISDOM` -> 468
- `AN INSTRUCTION` -> 520

So the rule is not simply “nearby text tends to be prime”.

A 200,000-replay descriptive calibration preserving statement lengths and sampling from the pooled rune composition produced:

- mean prime count: `2.722405 / 17`
- maximum: 11
- 0 / 200,000 replays with all 17 prime

Because the external prime-GP lead was known before EXP-275, this is **not** presented as an unbiased discovery p-value.

## EXP-276 — not generic Runeglish prose

The prime property was compared against ordinary solved prose.

The special role-conditioned statements remained strongly enriched relative to the comparison class; the recorded comparison was `17/17` versus `18/58`, Fisher `p≈1.53×10^-7`.

This rejects the simple claim that prime sums are generic to solved Runeglish sentences.

It also showed the initial role taxonomy was incomplete: `A WARNING` and `PARABLE` supplied additional prime-GP content statements.

## EXP-277 — prospective holdout

This is the most important strengthening step.

Before testing the held-out solved instruction, the prediction was frozen that its GP sum would be **prime**.

Held-out text:

`DO FOUR UNREASONABLE THINGS EACH DAY`

Observed GP sum:

`1229`

`1229` is prime.

**SIGNAL STRONG — prospective replication.**

Important scope correction: the exact value **1229 was not prospectively predicted**. Only primality was.

## EXP-279 — source-only role taxonomy

A source-derived taxonomy, without GP-informed boundary edits, reconstructed 30 special content statements:

- 9 `A WARNING`
- 10 `WIDSOM` / `SOME WISDOM`
- 8 `AN INSTRUCTION`
- 3 `PARABLE`

This is **ESTABLISHED documentary coherence**.

The broader historical/community prime observations are corroborated, but no single pinned historical artifact was recovered that explicitly enumerates one complete external `30/30` inventory. Exact identity with such a remembered inventory remains **OPEN**.

## EXP-280 — how strong is the checksum?

The 30 frozen statements were perturbed exhaustively using one-word substitutions drawn from their own 89-word vocabulary.

Primary enumeration:

- substitutions: **12,760**
- prime-result substitutions: **1,790**
- fraction remaining prime: **0.140282**
- about **85.97%** of arbitrary one-word edits break primality
- every one of the 30 statements nevertheless has at least one prime-preserving alternative
- median random edits to encounter a prime-preserving variant: about **7.16**

Same-rune-length replacement restriction:

- substitutions: 1,768
- prime-result substitutions: 425
- prime fraction: `0.24038`

Interpretation:

> Prime-GP is selective enough to act as a lightweight downstream authorial verifier, but far too easy to satisfy deliberately to function as a unique cryptographic authenticator.

## Rubrication is complementary, not identical

EXP-451 tested a tempting cross-domain interpretation: perhaps red text marks the prime-GP statements directly.

It failed.

On solved material, red spans repeatedly mark titles, short labels and structural framing, while multiple prime-GP content statements are black.

**REJECTED scoped:** `red -> prime statement`.

**SIGNAL:** rubrication may preferentially mark a structural/meta layer, complementary to the semantic prime-GP layer.

This distinction motivates future document-architecture work.

## Correct use

Prime-GP should be used only in this order:

1. obtain a candidate plaintext independently;
2. obtain its semantic role and boundaries independently;
3. then test whether the role-conditioned statement obeys the prime-GP convention.

Do **not** search wording until a prime appears. That reverses the evidential direction and makes the property easy to manufacture.

## Current interpretation

- `ESTABLISHED`: source-defined solved statement classes show the prime-GP relation.
- `SIGNAL STRONG`: the relation behaves like an intended lightweight verifier/stylistic checksum.
- `OPEN`: whether analogous role classes exist in unresolved LP2.
- `REJECTED`: prime-GP as direct LP2 decoder/key/offset/keystream.
