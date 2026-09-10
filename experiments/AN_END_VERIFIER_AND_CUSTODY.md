# AN END — verifier, serialization and historical custody

## What the solved text actually establishes

The solved terminal page says, in substance, that within the deep web there exists a page that hashes to the published hexadecimal value, and that pilgrims should seek it.

Frozen target:

`36367763ab73783c7af284446c59466b4cd653239a311cb7116d4618dee09a8425893dc7500b464fdaf1672d7bef5e891c6e2274568926a49fb4f45132c2a8b4`

The value is:

- 128 hexadecimal characters
- 64 bytes
- 512 bits

**ESTABLISHED:** the text asserts a page-to-hash relation.

## What it does not establish

The source does not name:

- SHA-512;
- the exact bytes that are hashed;
- URL vs hostname vs path vs HTTP response vs body vs file vs normalized text;
- newline/charset/decompression/rendering normalization;
- Tor or `.onion` specifically;
- a locator encoded directly in the 512-bit object.

Therefore these remain **OPEN** unless independently fixed.

## Why brute-force normalization is methodologically weak

Given a candidate page, there are many plausible representations. Trying algorithms, URLs, body extractions, charsets, newline conventions and decompression rules until something matches creates a large hidden search space.

The project therefore adopted a strict rule:

> freeze the historical object and its representation before target-bearing digest comparison.

## Historical hash convention audit

A bounded audit of preserved 2012–2014 Cicada material found repeated OpenPGP clearsigned messages using `Hash: SHA1`.

This establishes a genuine historical convention for **OpenPGP cleartext authentication**, but not an AN END page serialization convention.

**REJECTED scoped:** historical Cicada material independently fixes AN END serialization.

**REJECTED claim:** OpenPGP SHA1 precedent licenses choosing a page representation or `SHA-512(raw body)` for AN END.

## Freenet CHK test

A constrained alternative interpretation was tested: perhaps the 64-byte object directly encodes a Freenet CHK locator.

A 2014 Freenet CHK includes:

- 32-byte routing key;
- 32-byte crypto key;
- an additional 5-byte `extra` field carrying required semantics such as algorithm/control/compression state.

The AN END object supplies the first 64 bytes but not a uniquely determined `extra` field.

**REJECTED scoped:** the 512-bit object alone deterministically specifies one complete Freenet 0.7 CHK.

The superficial `32+32` resemblance remains only **COINCIDENCE / OPEN compatibility**.

## Historical custody work

Rather than enumerate candidate pages blindly, the project searched for historically relevant collections that could have preserved early hidden-service content.

After deduplication, the strongest operator/data-custody routes were:

1. TNO / Dark Web Monitor lineage
2. Portsmouth / early Tor crawl research lineage
3. DARPA Memex / SRI LIGHTS
4. Moore / Rid 2015 crawl corpus

A later DUTA author-held corpus remains secondary/open.

This list describes **historically plausible custody**, not evidence that any collection contains the target page.

A bounded follow-up search did not recover another independently justified public route. Several preservation inquiries have not produced actionable data; future progress should not depend on repeated unsolicited contact.

## Current status

- page-to-hash semantics: **ESTABLISHED**
- exact 512-bit target: **ESTABLISHED**
- algorithm: **OPEN**
- exact serialization/input representation: **OPEN**
- locator/service: **OPEN**
- historical object custody: **OPEN**
- `SHA-512(raw page body)` as source-established rule: **REJECTED claim**
- deterministic complete Freenet CHK: **REJECTED scoped**

## What would materially advance this problem

High-value evidence would be one of:

- an exact dated 2014 hidden-service snapshot/export with provenance;
- an old solver archive containing the relevant retrieved page/object;
- an authenticated source instruction fixing the representation or hash algorithm;
- a preserved crawler record whose storage semantics are documented precisely enough to define deterministic bytes.

Without one of those, another large hash/normalization sweep is more likely to generate false confidence than knowledge.
