---
title: Frequency Analysis
created: 2026-07-20
updated: 2026-07-20
type: concept
tags: [cryptography, frequency-analysis, cryptanalysis, wilkins, cipher-breaking, 17th-century]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Frequency Analysis in Cryptology

**Frequency analysis** is the fundamental technique of classical cryptanalysis — the method of breaking substitution ciphers by analysing how often each symbol appears in the ciphertext and matching those frequencies to known letter distributions in the target language. [John Wilkins](entities/john-wilkins.md) provides one of the earliest English-language descriptions of the method in [Chapter 11](concepts/ch-11-invented-characters.md) of [*Mercury*](entities/mercury-wilkins.md) (1641), predating the better-known treatments by nearly a century.

## The Principle

Every written language has a characteristic frequency distribution of letters. In English, for example:

- **E** is by far the most common letter (~12.7%)
- **T, A, O, I, N, S, H, R** follow (~6–9% each)
- **D, L, C, U, M, W, F, G, Y, P, B** are mid-frequency (~1.5–4%)
- **V, K, J, X, Q, Z** are rare (<0.5% each)

A monoalphabetic substitution cipher preserves these frequencies — it merely replaces each letter with a different symbol (or another letter). The most frequent symbol in the ciphertext is therefore almost certainly the symbol for **E**; the second most frequent is probably **T**; and so on.

## History Before Wilkins

### Arab Cryptologists (9th Century)

Frequency analysis was first developed by **Arab scholars** in the Abbasid Caliphate. The polymath **Al-Kindi** (c. 801–873) described the technique in his *Risāla fī Istikhrāj al-Muʿammā* ("Manuscript on Deciphering Cryptographic Messages") — the earliest known treatise on cryptanalysis. Al-Kindi's method:

1. Count the frequency of each ciphertext symbol
2. Identify the most frequent as the symbol for the most frequent letter in the target language
3. Work through decreasing frequencies
4. Use knowledge of common words, digraphs, and trigraphs to resolve ambiguities

This knowledge passed into the Islamic cryptographic tradition and fundamentally undermined the security of monoalphabetic substitution — though it did not reach Western Europe until centuries later.

### Porta (1563)

[Giambattista della Porta](entities/porta-baptista.md) described frequency-based cryptanalysis in *De Furtivis Literarum Notis* (1563), providing systematic rules for Italian and Latin. Wilkins explicitly credits Porta as a source: "you may see them largely handled by Baptista Porta, and Gustavus Selenus."

### Selenus (1624)

Gustavus Selenus (pseudonym of Augustus the Younger, Duke of Brunswick-Lüneburg) included extensive frequency tables in *Cryptomenytices et Cryptographiae* (1624). He provided letter frequency data for Latin, German, and Italian — the most thorough pre-Wilkins treatment.

## Wilkins's Method (Chapter 11)

Wilkins presents frequency analysis as the method for **unfolding** (breaking) the geometrical and invented-character ciphers he has just described. His method is practical, systematic, and addressed to the English reader:

### Step 1: Identify the Vowels

> "Endeavour to distinguish betwixt the vowels and consonants. The vowels may be known by their frequency, there being no word without some of them."

Vowels appear in **every word** — this is invariant across languages. If a ciphertext symbol appears in every word, it is almost certainly a vowel.

### Step 2: Single Characters Must Be A, I, or O

> "If there be any single character in English, it must be one of these three vowels, A, I, O."

This is an English-specific positional rule: in English, the only one-letter words are "a" and "I" (and the interjection "O"). Any ciphertext symbol that appears alone must represent one of these.

### Step 3: Letter Frequency Tables

> "Search after the several powers of the letters: for the understanding of this, you must mark which of them are most common, and which more seldom used."

Wilkins makes a practical suggestion: consult **printers**:

> "This the printers in any language can easily inform you of, who do accordingly provide their sets of letters."

Printers knew letter frequencies because they needed to **stock type** in proportion to use — more E's than Z's. This is an inspired connection between industrial practice and cryptographic theory: the compositor's type case *is* a frequency table.

### Step 4: Doubled Letter Rules

Certain letters are never doubled in English: **H, Q, X, Y**. If a ciphertext symbol is doubled, it cannot be one of these. Conversely, **L, S, E, O, F** are commonly doubled (*ball*, *pass*, *see*, *too*, *off*).

### Step 5: Positional Tables

Wilkins recommends constructing tables of:

- "The number of vowels or consonants in the beginning, middle, or end of words"
- Two-letter word patterns: vowel-consonant (*am, an, as, if, in, is, it, of, on, or, us*) vs. consonant-vowel (*be, he, me, by, my, do, to, so*)

"These tables must be various, according to the difference of languages."

### Step 6: Resolve by Context

> "You may thereby the easier guess at any disguised sense."

Once enough letters are identified, the plaintext emerges through word recognition — the same human pattern-matching that makes crosswords solvable.

## Countermeasures: How to Defeat Frequency Analysis

Wilkins acknowledges that frequency analysis is powerful but not invincible. He immediately provides countermeasures:

> "The common rules of unfolding being once known, a man may the better tell how to delude them."

1. **Double-represent vowels**: Assign the rare letters' characters (H, K, Q, X, Y) as *second symbols* for vowels — so each vowel gets two possible representations, flattening the frequency distribution.

2. **Write continuously**: Eliminate spaces between words, destroying the positional cues (single-character words, word boundaries).

3. **Insert false word breaks**: Deliberately place spaces at wrong positions.

4. **Insert nulls**: Add non-significant characters that don't map to anything.

These four countermeasures anticipate the development of **polyalphabetic ciphers** — the next major advance in cryptographic security — which Wilkins had already described in [Chapter 7](concepts/ch-7-equal-letters-powers.md) (the key-character cipher). Wilkins is unusual among early cryptographers in presenting both the lock (the cipher) and the key (frequency analysis) in the same book.

## Historical Significance

Wilkins's frequency analysis section is one of the **earliest English-language descriptions** of systematic cryptanalysis. The timeline:

| Date | Author | Contribution |
|------|--------|-------------|
| c. 850 | Al-Kindi | First description (Arabic) |
| 1563 | Porta | First Western treatment (Latin, Italian) |
| 1624 | Selenus | Frequency tables for Latin, German, Italian |
| **1641** | **Wilkins** | **First English-language treatment** |
| 1711 | John Falconer | *Cryptomenysis Patefacta* (English, full frequency tables) |

Wilkins does not provide comprehensive frequency tables — he defers to Porta and Selenus for those — but his methodological framework is clear, practical, and explicitly designed for the English reader. His printer's-type suggestion is a genuinely original contribution.

## Cross-References

- [ch-11-invented-characters](concepts/ch-11-invented-characters.md) — the chapter where Wilkins presents frequency analysis
- [ch-7-equal-letters-powers](concepts/ch-7-equal-letters-powers.md) — the polyalphabetic cipher (countermeasure)
- [mercury-wilkins](entities/mercury-wilkins.md) — the book
- [porta-baptista](entities/porta-baptista.md) — Wilkins's cited source on frequency analysis
- [atbash](concepts/atbash.md) — the simplest substitution cipher vulnerable to frequency analysis
