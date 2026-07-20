# Wiki Log — Crypto-History

> Chronological record of all wiki actions. Append-only.
> Format: `## [YYYY-MM-DD] action | subject`

## [2026-07-20] create | Wiki initialized

- Domain: History of cryptography, centered on John Wilkins's *Mercury* (1641)
- Structure created: SCHEMA.md, index.md, log.md
- Sources ingested: mercury-1694.pdf (Gallaudet copy, 12MB), mercury-1802.txt (clean OCR, 616KB)
- Wiki directory: /opt/data/home/wiki/crypto-history/

## [2026-07-20] ingest | Mercury: or the Secret and Swift Messenger (Wilkins, 1641/1694/1802)

**Sources:**
- Downloaded 1694 edition PDF from Internet Archive (Gallaudet University copy)
- Downloaded 1802 edition plain text from Internet Archive (Mathematical Works Vol. II)

**Pages created (entities):**
- entities/mercury-wilkins.md — comprehensive book overview
- entities/john-wilkins.md — author biography
- entities/polybius-cipher.md — the Polybius cipher system
- entities/francis-godwin.md — Godwin and *Nuntius Inanimatus*

**Pages created (chapters):**
- concepts/ch-1-dependence-in-nature.md through concepts/ch-20-polybius-torch-cipher.md
- concepts/conclusion-moral-defense.md

**Pages created (supporting concepts):** (in progress)

**Structural files:**
- SCHEMA.md — conventions, tag taxonomy, page thresholds
- index.md — complete content catalog
- log.md — this file

## [2026-07-20] lint | Initial link audit

- Fixed 10 broken wikilinks (naming mismatches: ch-17-sound-signals→ch-17-joining-secrecy-swiftness-sound, etc.)
- Identified ~18 missing linked pages — dispatched subagent to create them
