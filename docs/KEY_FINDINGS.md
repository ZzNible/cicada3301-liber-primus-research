# Key Findings

This document highlights results that survived correction, replay, provenance checks, or dependency repair.

## 1. The low immediate-repeat count is real

**SIGNAL**

In the canonical unresolved LP2 rune stream:

- runes: `12,956`;
- valid adjacent transitions: `12,954`;
- immediate self-repeats: `86`.

The low repeat count is not explained by known transcription/page-assignment mistakes, punctuation proximity, line/page resets, or rubricated-runic regions in the tested scopes.

The mechanism remains **OPEN**.

## 2. Several apparent supporting anomalies are not independent

**ESTABLISHED methodological correction**

The observations that every diagonal transition cell is a row minimum, and that self-repeat ranks remain low across temporal folds, initially looked like additional evidence.

Fixed-repeat-count null replays showed that both are common once `K=86` is conditioned on.

Therefore these observations must not be multiplied together as independent evidence.

## 3. Simple anti-repeat generators do not explain LP2

**REJECTED scoped**

- A pure Goldman-style no-repeat generator would force `K=0`, not 86.
- A simple uniform max-run-2 generator naturally produces far more repeated transitions than observed; the LP2 repeat count is extremely far into its lower tail.

A fixed-K enumerative model can reproduce the count by construction, but that is **OPEN / compatible only** and not evidence that Cicada used such a code.

## 4. Cross-round semantic/representation reuse exists

**ESTABLISHED scoped**

A preserved 2012 phrase, `Patience is a virtue`, maps under Gematria Primus to `761`. The number `761` later appears as a deliberate 2014 marker.

This demonstrates that Cicada can reuse semantic/representation material across campaigns.

It does not establish arbitrary byte-level reuse of earlier files.

## 5. CicadaOS is historically relevant, but not an LP2 key by default

**ESTABLISHED historical provenance**

The 2013 CicadaOS path is real and the roles of `_560.00`, `560.13`, and `560.17` are historically documented.

**REJECTED scoped**

No bounded authenticated/pinned 2014 source prescription was found that deterministically selects those bytes as LP2 input.

## 6. AN END is a real page-to-hash instruction

**ESTABLISHED**

The solved wording says that a page in the deep web `HASHES TO` the exact published 512-bit value.

This corrects a weaker interpretation in which the page and value might merely have been juxtaposed.

However, the text does not itself specify SHA-512, exact serialized bytes, URL syntax, page body, newline convention, or normalization.

## 7. Historical hashing precedent does not fix AN END serialization

**ESTABLISHED + REJECTED scoped**

Cicada repeatedly used OpenPGP cleartext signatures with SHA1 in historical campaigns.

That is a real repeated protocol convention, but it does not transfer automatically to the `AN END` page-hash verifier.

## 8. AN END is now primarily a custody problem

**ESTABLISHED integration / OPEN recovery**

After deduplication, four primary historically plausible custody routes remain:

1. TNO / Dark Web Monitor;
2. Portsmouth / Searchlight Cyber;
3. DARPA Memex / SRI LIGHTS;
4. Moore / Rid 2015.

No additional fifth route was recovered from the already-audited canonical source set.

## 9. Public source repositories are not currently hiding an obvious missing key object

**OPEN / bounded negative**

A frozen audit of resolvable public repository families recovered no new qualifying 2012–2014 Cicada source object capable of reopening the current LP2 or AN END holds.

This does not exclude deleted repositories, private solver archives, recipient-only material or operator datasets.

## 10. Current scientific conclusion

No unknown LP2 plaintext is established.

The strongest next move is not a larger brute-force search. It is obtaining genuinely new authenticated evidence that fixes a mechanism, object or representation before testing it against LP2.