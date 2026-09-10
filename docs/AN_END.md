# AN END — What Is Actually Established?

The solved Liber Primus section `AN END` contains one of the clearest externally verifiable instructions in the book.

## Established wording-level fact

**ESTABLISHED:** the solved text states that, within the deep web, there exists a page that `HASHES TO` the published 512-bit value, and that pilgrims should seek that page.

Frozen target:

`36367763ab73783c7af284446c59466b4cd653239a311cb7116d4618dee09a8425893dc7500b464fdaf1672d7bef5e891c6e2274568926a49fb4f45132c2a8b4`

The target is 128 hexadecimal characters = 64 bytes = 512 bits.

## What the source does not establish

**OPEN:**

- the hash algorithm;
- whether the input is a URL, hostname, path, HTTP response, HTML body, downloaded file, text extraction, or another representation;
- normalization, whitespace/newlines, encoding, decompression, headers or rendering;
- whether `deep web` specifically means Tor/.onion;
- the exact historical object or service;
- whether the page still exists publicly.

**REJECTED claim:** the target length alone proves SHA-512.

## Historical convention audit

Cicada repeatedly used OpenPGP cleartext signatures with SHA1 in preserved 2012 and 2014 messages.

That is an **ESTABLISHED historical convention** for the OpenPGP object class.

It does not independently fix the representation or algorithm used by the `AN END` verifier. Transfer of that convention is therefore **OPEN / unsupported**, not evidence for SHA1 or SHA-512 over a guessed page representation.

## Why this became a custody problem

Blindly enumerating hash algorithms and page normalizations creates an enormous look-elsewhere problem. A matching digest would only be persuasive if the candidate object and representation were fixed independently.

Historical archive research therefore shifted from "try hashes" to "recover the exact object or a source-defined representation".

After deduplication, four primary operator-gated historical routes remain:

1. **TNO / Dark Web Monitor** — direct lineage to Tor crawling beginning in 2013; exact 2014 survival/representation remains open.
2. **Portsmouth / Gareth Owenson / Searchlight Cyber** — historically relevant 2014 research/crawling lineage; raw corpus survival remains open.
3. **DARPA Memex / SRI LIGHTS** — 2014+ onion crawling and later preserved snapshot lineage; historical export survival and page semantics remain open.
4. **Moore / Rid 2015** — large Jan–Mar 2015 Tor crawl with a MongoDB-backed corpus; survival/export remains open.

DUTA-private remains a secondary possibility because author-held historical content may survive even though public DUTA is not deterministic historical custody.

## Reopening criterion

Digest testing should resume only if at least one of the following appears:

- an exact historical page/object;
- a dated archive member with preserved bytes;
- a custodian-provided dataset/export;
- a source-defined locator;
- a source-defined representation/serialization rule.

Freeze provenance and representation **before** computing candidate digests.