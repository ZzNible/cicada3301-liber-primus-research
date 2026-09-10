# Cicada 3301 / Liber Primus Research

Independent, evidence-driven research on Cicada 3301 and the unresolved pages of the **Liber Primus**.

> **Current status:** the unsolved Liber Primus has **not** been decrypted by this project. No unknown plaintext is claimed.

This repository publishes a curated subset of a larger private research lab. Its purpose is to help the community distinguish:

- reproduced facts from speculation;
- real statistical signals from dependent or post-hoc effects;
- promising open questions from already-tested dead ends;
- primary/authenticated material from mirrors, transcriptions and solver folklore.

## Status vocabulary

Every important claim is labelled explicitly:

- **ESTABLISHED** — reproduced, verified and documented;
- **SIGNAL** — a measured anomaly is real, but its interpretation is not established;
- **HYPOTHESIS** — a precise explanation with a falsifiable test;
- **OPEN** — compatible with the evidence, without positive proof;
- **REJECTED** — falsified within a clearly stated scope;
- **COINCIDENCE** — intriguing relation without established intentionality/significance.

## Current high-level result

The strongest local ciphertext observation in our canonical LP2 corpus is a low number of immediate repeated runes:

- canonical unknown LP2 stream: **12,956 GP runes**;
- valid adjacent transitions: **12,954**;
- immediate self-repeats: **86**.

This is a **SIGNAL**. The mechanism remains **OPEN**.

Several visually striking secondary patterns initially appeared to support the same story, but controlled fixed-K replays showed that they do **not** provide strong independent evidence once the 86 repeats are conditioned on. This is one of the main methodological corrections produced by the project.

## Other important findings

- **Cross-round reuse is real in at least one documented case.** `Patience is a virtue` from 2012 maps through Gematria Primus to **761**, and 761 is deliberately reused as a 2014 marker. This establishes semantic/representation reuse across campaigns, but does not justify arbitrary reuse of old files as LP2 keys.
- **CicadaOS 2013 provenance is historically real**, including the roles of `_560.00`, `560.13` and `560.17`; however, no authenticated 2014 source was found that prescribes those bytes as an LP2 pad/input.
- **AN END really says that a page in the deep web hashes to the published 512-bit value.** The source does **not** identify SHA-512, exact input bytes, URL/body/file representation, or normalization.
- Historical custody research for `AN END` currently concentrates on four operator-gated routes: TNO/Dark Web Monitor, Portsmouth/Searchlight, SRI/Memex, and Moore/Rid.
- A bounded audit of public source repositories recovered **no new qualifying 2012–2014 primary object** able to reopen the current holds.

## Selected experiment chains

The public repository now includes concise, reusable summaries of the most important experiment chains:

- [`experiments/K86_TRANSITION_SIGNAL.md`](experiments/K86_TRANSITION_SIGNAL.md) — the repeat-suppression signal and failed explanations;
- [`experiments/PRIME_GP_VERIFIER.md`](experiments/PRIME_GP_VERIFIER.md) — the prime-GP solved-plaintext verifier and prospective holdout;
- [`experiments/AN_END_VERIFIER_AND_CUSTODY.md`](experiments/AN_END_VERIFIER_AND_CUSTODY.md) — page-to-hash semantics, representation limits and custody work;
- [`experiments/MIXED_DOCUMENT_ARCHITECTURE.md`](experiments/MIXED_DOCUMENT_ARCHITECTURE.md) — the layered data/control/verification framing.

See [`experiments/README.md`](experiments/README.md) for the curated experiment index.

## Why so many negative results?

Because publishing them saves the community time.

This project deliberately records failed families instead of silently discarding them. A negative result is useful only when its scope is clear, the search degrees of freedom are accounted for, and the test has a meaningful positive control.

See:

- [`docs/CURRENT_STATE.md`](docs/CURRENT_STATE.md)
- [`docs/KEY_FINDINGS.md`](docs/KEY_FINDINGS.md)
- [`docs/NEGATIVE_RESULTS.md`](docs/NEGATIVE_RESULTS.md)
- [`docs/AN_END.md`](docs/AN_END.md)
- [`docs/METHODOLOGY.md`](docs/METHODOLOGY.md)
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md)

## Research posture

As of September 2026 the project is **evidence-gated, not compute-gated**.

We do **not** recommend opening another large parameter sweep over the known ciphertext. The most valuable next input would be new authenticated evidence: an old solver archive, a preserved onion snapshot, a private 2014 recipient object, an operator dataset, a source-defined representation rule, or a historically anchored mechanism that makes a new prediction before LP2 is inspected.

## About Pliny / Plinius

No historical link between Cicada 3301 and **Pliny the Elder** or the contemporary LLM-jailbreak researcher **Pliny the Liberator** is established.

There are, however, two useful analogies:

- **HYPOTHESIS / structural analogy:** Book I of Pliny the Elder's *Natural History* functions largely as a contents/source map rather than ordinary exposition. This invites a falsifiable reading of *Liber Primus* as potentially containing routing/indexing/meta-instructions rather than being only a homogeneous ciphertext stream.
- **OPEN / methodological analogy:** decomposition, representation changes, boundary probing and recomposition — techniques associated with modern LLM jailbreak research — are useful research tactics for Cicada, but do not constitute historical evidence of a connection.

These analogies are kept separate from established Cicada evidence.

## Provenance and redistribution

This repository does not blindly mirror the private lab or third-party archives. Primary artifacts remain attributed to their original sources; files with unclear redistribution status are referenced rather than republished.

The private working repository remains the canonical research source. This public repository is a curated publication layer.
