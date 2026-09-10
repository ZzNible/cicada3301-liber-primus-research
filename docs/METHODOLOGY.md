# Methodology

The project treats Cicada 3301 / Liber Primus as a research problem, not a word-hunting contest.

## Core rule

A result is only interesting if the search process that produced it is auditable.

Before an important experiment we aim to freeze:

- the hypothesis;
- the exact prediction;
- corpus and provenance;
- hashes of relevant inputs;
- parameters chosen before calculation;
- primary metric;
- null model;
- multiple-search/look-elsewhere correction;
- positive control;
- rejection/continuation criterion;
- explored degrees of freedom.

## Null models must replay the search

If an experiment searches many offsets, directions, transforms or parameter values and reports the best one, the null must reproduce that complete search process.

Comparing only the selected winner against a single unsearched random baseline badly understates false-positive probability.

## Positive controls

A detector that fails on the real data proves little unless we know it could detect the hypothesized mechanism when present.

Whenever practical, we therefore use:

- solved historical Cicada material with a known mechanism; or
- synthetic data generated with the mechanism being tested.

If the positive control lacks power, the correct conclusion is usually **OPEN / INCONCLUSIVE**, not `REJECTED`.

## Dependency repair

Multiple statistics derived from the same underlying feature must not be counted as independent evidence.

The `K=86` investigation is an important example. Row-minimum and temporal-floor effects initially looked independently remarkable. Once the null fixed the observed repeat count, those effects became common.

This converted an apparently multi-signal story into one primary signal plus downstream consequences.

## Corpus discipline

We separate:

- primary artifacts;
- historical copies;
- community transcriptions;
- canonical analysis corpus;
- derived datasets;
- experiment outputs.

A transcription is not lossless merely because rune identities match: layout, color, separators, punctuation and marginalia can carry information.

Primary artifacts are never silently modified.

## Source evidence vs solver hypotheses

A mechanism implemented in community code is evidence that a solver considered it, not evidence that Cicada used it.

We explicitly distinguish:

- source-authored instruction;
- historically preserved puzzle object;
- community reconstruction;
- modern solver tooling;
- our own hypothesis.

## Status vocabulary

- `ESTABLISHED`: reproduced, verified and documented.
- `SIGNAL`: measured anomaly; interpretation not established.
- `HYPOTHESIS`: precise explanation with falsifiable test.
- `OPEN`: compatible with evidence without positive proof.
- `REJECTED`: falsified in a clearly defined domain.
- `COINCIDENCE`: intriguing relationship without established intention/significance.

## What we deliberately avoid

We do not accept an English-looking local fragment when:

- the full page/block remains random;
- parameters were optimized after seeing the output;
- the fragment depends on manual selection;
- the search does not survive look-elsewhere correction.

Nor do we optimize arbitrary offsets, alphabets, directions, inversions, permutations or constants until a desirable phrase appears.

## When a wild idea is welcome

Unconventional ideas are useful when they generate a new prediction.

A productive "crazy idea" should therefore be:

1. stated precisely;
2. falsifiable;
3. tested against controls;
4. abandoned or downgraded if it fails.

The goal is cumulative knowledge, including reliable negative knowledge.