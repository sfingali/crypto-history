---
title: "Bacon vs Wilkins on Cryptography: Taxonomist vs Encyclopaedist"
created: 2026-07-20
updated: 2026-07-20
type: comparison
tags: [comparison, bacon, wilkins, cryptography, biliteral-cipher, taxonomy, encyclopaedia, 17th-century]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Bacon vs Wilkins on Cryptography: Taxonomist vs Encyclopaedist

**Francis Bacon** (1561–1626) and **John Wilkins** (1614–1672) both contributed to cryptography, but from fundamentally different positions. Bacon was a taxonomist who *noticed* cryptography as a gap; Wilkins was an encyclopaedist who *filled* it. Their relationship is not one of rivalry but of foundation and fulfilment — Wilkins builds on Bacon's map of knowledge to construct the building Bacon only pointed to.

## The Relationship

Wilkins explicitly places himself in Bacon's intellectual lineage. In the introduction to *Mercury: or the Secret and Swift Messenger* (1641), he calls Bacon **"our English Aristotle"** and acknowledges that in *The Advancement of Learning* (1605), Bacon "hath briefly contracted the whole substance of what may be said in this subject. Where he refers it to the art of Grammar, noting it as a **deficient part**." This phrase — "deficient part" — is the conceptual hinge between the two men. Bacon identified a gap; Wilkins resolved to fill it.

## Dimensions of Comparison

| Dimension | Francis Bacon | John Wilkins |
|-----------|--------------|--------------|
| **Context** | *The Advancement of Learning* (1605), *De Augmentis Scientiarum* (1623) — comprehensive taxonomies of all human knowledge | *Mercury: or the Secret and Swift Messenger* (1641) — a book entirely devoted to cryptography and secret communication |
| **Cryptography's place** | A sub-section of Grammar, under the "organ of speech" — one entry in an encyclopaedia of all the sciences | The centrepiece — the entire book treats ciphers, steganography, signals, and universal characters as a unified field |
| **Method** | Taxonomic classification: where does this fit in the tree of knowledge? | Encyclopaedic collection: what are all the things people have done in this domain? |
| **Primary cipher contribution** | The **biliteral cipher** — a binary encoding system of elegant theoretical simplicity. Any letter expressed as 5 `a`/`b` values (2⁵ = 32). Hidden via two typefaces. | Multiple cipher systems: substitution with equal/more/fewer letters, transposition, invented characters, key-character systems. Practical adaptability over theoretical elegance. |
| **Treatment of the biliteral cipher** | Originator. Described in *De Augmentis* Book 6, Chapter 8. | Explainer and extender. Discusses it in [Chapter 9](concepts/ch-9-barbarous-words.md) as one instance of the general principle that any alphabet can be reduced to two symbols. Connects it to the torch telegraph of [Chapter 20](concepts/ch-20-polybius-torch-cipher.md). |
| **Tone and audience** | Philosophical, addressed to James I — a statesman-philosopher mapping the intellectual world for the benefit of a monarch | Practical, addressed to "statesmen and soldiers" — a working clergyman equipping men of action with useful knowledge |
| **Relationship to magic** | Rejected magic as part of his reform of natural philosophy — the "Idols of the Theatre" | Carefully distinguished genuine cryptography from "magical, or fabulous" traditions, cataloguing both while demarcating the boundary between science and credulity |
| **Universal language vision** | Speculated about "characters that express neither letters nor words, but things and notions" — a "real character" — as a possibility | Made the universal character the subject of [Chapter 13](concepts/ch-13-universal-character.md) of *Mercury* and spent 27 years developing it into the *Essay towards a Real Character* (1668) |
| **Historical range** | Drew mainly on classical precedent; his bibliographic sources were limited | Exhaustively cited classical, medieval, and Renaissance sources — [Trithemius](entities/trithemius.md), [Porta](entities/porta-baptista.md), Selenus, [Bede](entities/bede.md), [Josephus](entities/josephus.md), and dozens more |

## The Biliteral Cipher: Theory Becomes Practice

Bacon's biliteral cipher is his most famous cryptographic contribution — and its elegance is undeniable. The key insight is binary: **any letter of the alphabet can be expressed as a combination of only two symbols** (`a` and `b`) in groups of five. Since 2⁵ = 32, five binary positions can represent 24 letters (I/J and U/V conflated).

The genius was in the hiding. Bacon proposed using two different **typefaces** within an innocent-looking text — Roman type for `a`, Italic for `b`, or any binary distinction: uppercase/lowercase, different inks, subtly different letter heights. This is what Bacon called writing *omnia per omnia* ("anything by anything") — "the highest degree of this ciphering."

Wilkins presents the biliteral cipher in Chapter 9 not as the pinnacle of cryptography but as one technique among many. He shows how the same binary principle applies to the **torch telegraph** (two torches raised in sequence encoding any letter) and the **bell-and-trumpet** system (two distinct sounds). The biliteral cipher, in Wilkins's hands, becomes not a standalone curiosity but a **general principle**: any communication medium with at least two distinguishable states can encode the entire alphabet.

Where Bacon gave the world a brilliant idea, Wilkins showed how to *use* it — and how it connected to other ideas.

## How Mercury Fulfills Bacon's "Deficient Part"

Bacon classified cryptography under Grammar as a "deficient part" — meaning the art existed but hadn't been properly systematised. His own treatment of it, as Wilkins notes, "briefly contracted the whole substance of what may be said" — a sketch, not a treatise.

*Mercury* fulfills Bacon's call in several ways:

1. **Completeness**: Where Bacon offered a paragraph, Wilkins wrote a book. *Mercury* catalogs every known method — by materials, by form (equal letters, more letters, fewer letters, transposition), by invented characters, by signals, by gestures.

2. **Method**: *Mercury* is a **Baconian "natural history"** of cryptography — collecting, cataloguing, and comparing every known method before drawing conclusions. This is precisely the inductive method Bacon championed.

3. **Practical utility**: Bacon insisted knowledge should bear fruit in "works" — practical applications. Wilkins never loses sight of this: secrecy, speed, and reliability are the organising principles throughout.

4. **Demarcation**: Bacon's rejection of the "Idols" — systematic errors of thought — finds its echo in Wilkins's careful separation of genuine cryptographic technique from magical and fabulous claims (treated separately in [Chapter 19](concepts/ch-19-fabulous-magical.md)).

5. **The expansion of scope**: Bacon classified cryptography under Grammar. Wilkins expands it to encompass the full spectrum of communication — speech, writing, and gesture — treating expression itself as currency: "expressions being current for conceits, as money is for valuations."

## Synthesis and Verdict

Bacon and Wilkins are complementary figures, not competitors. Bacon drew the map; Wilkins explored the territory. Bacon's biliteral cipher is a work of **theoretical genius** — a binary encoding system centuries ahead of its time, anticipating the logic of modern computing. Wilkins's *Mercury* is a work of **practical scholarship** — less conceptually original but far more useful to the statesman or soldier who needed to send a secret message tonight.

The relationship is captured in Wilkins's own framing: Bacon noted cryptography as a "deficient part" of Grammar. *Mercury* is the answer to that deficiency — the book that transforms a gap in the taxonomy of knowledge into a fully realised discipline. Without Bacon's classification, *Mercury* might not have been conceived as a work of systematic scholarship. Without *Mercury*, Bacon's classification would remain a footnote — an empty shelf in the library of learning.

The phrase "our English Aristotle" is not flattery. It is Wilkins's acknowledgment that his own work — encyclopaedic, systematic, practical — is what Bacon's method demanded. The taxonomist pointed to the gap; the encyclopaedist filled it.

## Cross-References

- [bacon-francis](entities/bacon-francis.md) — full entity page
- [john-wilkins](entities/john-wilkins.md) — full entity page
- [mercury-wilkins](entities/mercury-wilkins.md) — the book
- [ch-9-barbarous-words](concepts/ch-9-barbarous-words.md) — the biliteral cipher in *Mercury*
- [ch-13-universal-character](concepts/ch-13-universal-character.md) — the seed of the universal language
- [ch-20-polybius-torch-cipher](concepts/ch-20-polybius-torch-cipher.md) — the binary principle in telegraphy
- [bacon-cipher](concepts/bacon-cipher.md) — technical details of the biliteral cipher
- [universal-language-project](concepts/universal-language-project.md) — Wilkins's *Essay* as Baconian fulfilment
