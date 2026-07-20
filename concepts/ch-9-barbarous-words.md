---
title: "Chapter 9: Barbarous Words, Binary Encoding, and the Double Alphabet — The Best Kind of Secret Writing"
created: 2026-07-20
updated: 2026-07-20
type: concept
tags: [cryptography, wilkins, mercury, binary, encoding, bacon-cipher, double-alphabet, combinatorial]
book: mercury
chapter: 9
sources: [raw/mercury-1802.txt]
confidence: high
---

# Chapter 9: Barbarous Words, Binary Encoding, and the Double Alphabet

This is a **landmark chapter** in the history of cryptography and information theory. Here Wilkins presents the first systematic encoding of the alphabet into binary signals, the double alphabet (ancestor of Bacon's biliteral cipher), and their combination into what he calls "the best kind of secret writing."

## Barbarous Words: Only Some Letters Matter

The simplest method: write apparently nonsensical words where only the first, middle, and last letters are significant:

> *"Fildy, fagodur wyndeeldrare discogure rantibradi"*
> → *"Fly for we are discovered"*

The surrounding letters are padding — the secret resides in specific positions.

## Combinatorial Encoding: Any Five, Three, or Two Letters

This is the **intellectual breakthrough** of the chapter. Wilkins demonstrates that any alphabet can be encoded using a small number of symbols, simply by their repetition and order.

### Five-Letters Doubled (25 pairs)

> "All the letters may be expressed by any five of them doubled."

Using A, B, C, D, E as elements:

| Letter | Code | Letter | Code |
|--------|------|--------|------|
| A | aa | I | bd |
| B | ab | K | be |
| C | ac | L | ca |
| D | ad | M | cb |
| E | ae | N | cc |
| F | ba | O | cd |
| G | bb | P | ce |
| H | bc | ... | ... |

*"I am betrayed"* → *"Bd aacb abaedddbaaecaead"*

### Three-Letters Tripled (27 combinations, enough for alphabet)

Using A, B, C:

| Letter | Code | Letter | Code |
|--------|------|--------|------|
| A | aaa | M | ccb |
| B | aab | N | ccc |
| C | aac | O | aba |
| D | baa | P | abb |
| E | bba | Q | abc |
| ... | ... | ... | ... |

*"Hasten unto me"* → *"Caa aaa bca bcb bba abb bcc abb bcb abc aba bba"*

### Two-Letters Transposed Through Five Places (32 combinations)

> "Two letters of the alphabet being transposed through five places, will yield thirty-two differences, and so will more than serve for the four and twenty letters."

Using A and B:

| Letter | Code | Letter | Code |
|--------|------|--------|------|
| A | aaaaa | N | abbaa |
| B | aaaab | O | abbab |
| C | aaaba | P | abbba |
| D | aaabb | Q | abbbb |
| E | aabaa | R | baaaa |
| F | aabab | S | baaab |
| G | aabba | T | baaba |
| H | aabbb | V | baabb |
| I | abaaa | W | babaa |
| K | abaab | X | babab |
| L | ababa | Y | babba |
| M | ababb | Z | babbb |

This is a **pure binary encoding** — `AAAAA` = A, `AAAAB` = B, etc. It is mathematically identical to modern binary representation of 0–31 (the five-place table yields 2^5 = 32 values).

> *"Fly away"* → *"aababababababba aaaaabapaaaaaaababba"*

## The Double Alphabet

### Method

Create two alphabets visually similar but distinct — for example, Roman letters and italic letters (or as Wilkins describes, the second alphabet's letters being "more round and full than the other").

Write an innocent cover letter using mostly the first alphabet, but insert letters from the second alphabet to encode the secret message. Only the second-alphabet letters carry the hidden meaning.

### Example

Wilkins shows a letter from besieged soldiers with mixed Roman/italic type. The italic letters alone read: *"We perish with hunger; help us."*

### Improving Stealth

> "But because the differences betwixt these two alphabets may seem more easily discoverable, since they are both generally of the same kind... therefore for their better secrecy in this particular, it were safer to mix them both by compact, that they might not in themselves be distinguishable."

Distribute the two alphabets randomly among the letterforms — the appearance of difference is eliminated.

## The Master System: Double Alphabet × Binary Encoding

> "Now if this kind of writing be mixed with the latter way of secrecy, by two letters transposed through five places, we may then write *omnia per omnia* — which (as a learned man speaks) is the highest degree of this cyphering."

The **fusion**: each letter of the first alphabet = A; each letter of the second alphabet = B. Now any cover text of innocuous content carries a binary stream that encodes the full alphabet. Wilkins quotes Bacon's *Augmentis Scientiarum* (Book 6, chapter 8) — this is the **Baconian biliteral cipher**.

### Worked Example

A cover letter that superficially urges surrender:

> *"Send men, victuals, and all kind of necessaries for our sustenance, &c. As soon as you have received this, we shall be ready to meet you at the time and place appointed."*

The italic/roman pattern within it encodes:

> *"Fly, for we are discovered, I am forced to write this."*

Each group of 5 letters (type A or B) maps to one plaintext letter via the binary table.

### Triple Alphabet for Tighter Encoding

> "But now if there be a threefold alphabet (as is easy to contrive), then the inward writing will bear unto the outward but a triple proportion, which will be much more convenient for enlarging of the private intimations."

Three alphabets = ternary encoding = 3^5 = 243 combinations — vastly more efficient.

## Why This Is the Best System

Wilkins declares this combination meets all his criteria:

1. **Not laborious** to write or read
2. **Very difficult** to decipher by an enemy
3. **Void of suspicion** — the cover letter appears innocent

And for ultimate security:

> "It is to be generally observed, that the mixture of divers kinds of secret writing together (as suppose this with the key-character) will make the inward sense to be much more intricate and perplexed."

## Real-World Application: The Captive's Dilemma

Wilkins imagines a practical scenario:

> "Suppose a man were taken captive, he may by this means discover to his friends the secrets of the enemy's camp, under the outward form of a letter persuading them to yield. Or, suppose such a man were forced by his own hand-writing to betray his cause and party, though the words of it in common appearance may express what the enemy does desire; yet the involved meaning (which shall be legible only to his confederates), may contain any thing else which he has a mind to discover to them."

## Key Quotes

> "Two letters of the alphabet being transposed through five places, will yield thirty-two differences, and so will more than serve for the four and twenty letters."

> "We may then write omnia per omnia — which (as a learned man speaks) is the highest degree of this cyphering."

## Connections

- [[ch-7-equal-letters-powers]] — the key-character cipher, combinable with this method
- [[ch-8-more-letters]] — other methods of using more letters
- [[ch-17-joining-secrecy-swiftness-sound]] — binary encoding applied to bells and cannons
- [[polybius-cipher]] — binary/coordinate method applied to torches
- [[bacon-cipher]] — Bacon's biliteral cipher, directly referenced
- [[ch-20-polybius-torch-cipher]] — application to signal fires

## Diagrams in the Original

The 1694 edition contains woodcut tables for this chapter — among the earliest printed binary encoding tables:

![[assets/ch9-binary-alphabet.png]]
*Binary alphabet: any 2 letters transposed through 5 positions yield 32 combinations*

![[assets/ch9-double-alphabet.png]]
*Double-alphabet encoding grid with Latin example* ^[1802:5691-5920]
