---
title: SCHEMA
created: 2026-07-20
updated: 2026-07-20
type: meta
---

# Wiki Schema — Crypto-History

## Domain

Historical cryptography and secret communication, centred on John Wilkins's *Mercury: or the Secret and Swift Messenger* (1641) and its intellectual context. Extends to the history of ciphers, universal language projects, 17th-century science, and the Royal Society.

## Conventions

- **File names**: lowercase, hyphens for spaces (e.g., `ch-7-equal-letters-powers.md`, `john-wilkins.md`)
- **Link format**: Obsidian-compatible wikilinks (double-bracket notation)
- **Every page starts with YAML frontmatter** (title, created, updated, type, tags, sources, confidence)
- **Minimum 2 outbound links per page** (chapter pages aim for 3+)
- **When updating a page**, bump the `updated` date
- **Provenance**: key quotes from the 1802 text are cited inline. The `sources` field in frontmatter traces the page to `raw/mercury-1802.txt`

## Frontmatter

```yaml
---
title: Page Title
created: YYYY-MM-DD
updated: YYYY-MM-DD
type: entity | concept | meta | comparison | query
tags: [from taxonomy below]
sources: [raw/source-file.txt]
confidence: high | medium | low
---
```

## Tag Taxonomy

**Content tags:**
- `cryptography` — ciphers, codes, secret writing
- `cipher` — specific cipher systems (ATBASH, Caesar, Polybius, etc.)
- `substitution-cipher`, `transposition-cipher`, `steganography`
- `frequency-analysis` — cryptanalysis
- `signalling` — fire, smoke, bells, torches, semaphore
- `language` — linguistics, universal language, grammar
- `music` — musical ciphers and codes
- `gesture` — sign language, semaeologia

**People & institutions:**
- `wilkins` — John Wilkins specifically
- `mercury` — the book *Mercury*
- `bacon`, `porta`, `trithemius`, `godwin`, `leibniz`, `bede`
- `royal-society`

**Periods & contexts:**
- `17th-century` — the book's era
- `classical` — Greek and Roman sources (Polybius, Caesar, Josephus)
- `biblical` — Hebrew cabalistic ciphers
- `medieval` — Bede, Albertus Magnus, Roger Bacon

**Book structure:**
- `book: mercury` — marks the chapter pages
- `chapter: N` — chapter number

**Meta:**
- `meta` — wiki infrastructure pages
- `comparison` — side-by-side analyses

Rule: every tag on a page must appear in this taxonomy. Add new tags here before using them.

## Page Thresholds

- **Create a page** when an entity/concept appears in 2+ pages or is central to a chapter
- **Add to existing page** when a source mentions something already covered
- **DON'T create a page** for passing mentions
- **Split a page** when it exceeds ~200 lines

## Entity Pages

One page per notable person, book, or institution. Include:
- Overview / what it is
- Key facts and dates
- How it relates to Wilkins / *Mercury*
- Source references

## Concept Pages

One page per concept, cipher, or system. Include:
- Definition
- Technical explanation
- Historical context
- Connection to other chapters/concepts

## Chapter Pages

One page per chapter of *Mercury*. Include:
- Chapter number and title
- What it actually says (arguments, examples, references)
- Key quotes from the text
- Connections to other chapters

## Update Policy

When new information conflicts with existing content:
1. Check the dates — newer sources generally supersede older ones
2. If genuinely contradictory, note both positions with dates
3. Tag the contradiction
4. Flag for review
