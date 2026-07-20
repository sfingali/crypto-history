---
title: "Chapter 7: Secret Writing with Equal Letters by Changing Their Powers — ATBASH, Caesar, and the Key-Character"
created: 2026-07-20
updated: 2026-07-20
type: concept
tags: [cryptography, wilkins, mercury, substitution-cipher, caesar-cipher, atbash, key-character, cabala]
book: mercury
chapter: 7
sources: [raw/mercury-1802.txt]
confidence: high
---

# Chapter 7: Secret Writing by Changing the Powers of Letters

This is one of the most technically significant chapters in *Mercury*. Wilkins presents **substitution ciphers** — replacing letters with other letters — covering every known ancient and modern system, from Hebrew cabalistic ciphers to the key-character method that is the ancestor of the Vigenère cipher.

## The General Principle

> "As a written message may be concealed by changing the places of the letters, so likewise by changing of their powers, putting one of them for another, as suppose L for A, and A for L, or the like."

This is "answerable to that kind of cabalism in the Jewish learning, which the rabbies call *Ziruph*, or *combinatio*" — when alphabet letters are "severally transposed, and taken one for another, after any known order."

## Hebrew Cabalistic Ciphers

### Albam (אתבם)

Named from the first four corresponding letter pairs. Letters are paired from opposite halves of the alphabet (first with twelfth, second with thirteenth, etc.).

Wilkins gives its application: Isaiah 7:6 mentions a person under the name **Tabeal** (טבאל), whom the prophet says aspires to the crown of Judah. By this cabalism, the name is decoded — each letter replaced by its Albam partner — revealing **Remaliah** (רמליהו), the king of Israel, "whom he was loth more expressly to nominate."

### Athbash (אתבש)

Named from the first, last, second, and second-to-last letters. This is the reverse-alphabet substitution: א↔ת, ב↔ש, etc.

Wilkins gives its most famous application: Jeremiah 51:1, where the original text says **Leb kamai** (לב קמי, "the heart of those who rise against me"). By Athbash, לב becomes כשׁ — **Chasdim**, the Chaldeans. Both the Targum and the Septuagint "unanimously translate it so; as if in their version of it, they had chiefly respect unto this kind of cabalism."

Similarly, Jeremiah 51:41: the feigned name **Sheshach** (ששך) decodes by Athbash to **Babel** (בבל).

### Religious Significance

> "Both these kinds of secret writing, the Jewish doctors think to be frequently used by the sacred penmen of holy writ; amongst whom, the prophet Isaiah and Jeremiah are observed to be of more especial note for their skill in cabalisms."

## Roman Ciphers

### Julius Caesar's Cipher (Suetonius)

Caesar "when he would convey any private business, he did usually write it *per quartam elementorum literam*" — D for A, E for B, and so on. This is the **Caesar shift** of +3:

> *"Hasten unto me"* → *"Ldwxhq yqxr ph"*

### Augustus's Cipher

Octavius Augustus "did *secundum elementum proprii loco substituere*" — B for A, C for B, etc. (shift of +1). For A he used double X (xx).

## The Key-Character Cipher (Polyalphabetic Substitution)

Wilkins's most advanced contribution:

### The Problem with Single-Alphabet Ciphers

> "But now, because such an epistle might be easily unfolded, being altogether written by the same way; therefore this kind of secrecy hath, by later invention, been further obscured, by writing each several word, or line, or letter, by a diverse alphabet."

### The Solution: A Keyword as Key

Two friends agree upon a key word — "which words would be less discoverable, if they be barbarous, and of no signification." Wilkins's example uses the word **prudentia**.

For each letter of the keyword, a separate alphabet is constructed — each alphabet beginning with that letter. So:
- **P-alphabet**: P Q R S T V W X Y Z A B C D E F G H I K L M N O
- **R-alphabet**: R S T V W X Y Z A B C D E F G H I K L M N O P Q
- And so on through U, D, E, N, T, I, A

### Three Modes of Application

Wilkins shows the key-character can be applied:

1. **By lines**: Each line of ciphertext uses the next alphabet in sequence
2. **By words**: Each word uses the next alphabet
3. **By letters**: Each individual letter uses the next alphabet

He provides worked examples for all three, all encoding the message: *"The soldiers mutiny for want of victuals; supply us, or they will revolt to the enemy."*

### Further Obscurity: Mixed First Alphabet

> "These ways may be yet further obscured, if the first alphabet (according to which the rest are described) be contrived after any mixed order. As, suppose instead of the ordinary A B C, &c. there be written these letters, after this manner: *Rzkmpseblauftcygwhxoqind*."

This is equivalent to adding a **mixed alphabet** on top of the keyword — two layers of substitution. Wilkins notes this connects to "the wheel character... largely described by Porta" — foreshadowing the Porta cipher disk.

### The Infinite Variability

> "There may be divers other ways to this purpose, but by these you may sufficiently discern the nature of the rest."

## Key Quotes

> "This kind of secrecy hath, by later invention, been further obscured, by writing each several word, or line, or letter, by a diverse alphabet."

## Connections

- [ch-6-transposition](concepts/ch-6-transposition.md) — the other equal-letters method
- [ch-8-more-letters](concepts/ch-8-more-letters.md) — next method (more letters than needed)

## Diagrams in the Original

![Key-character alphabet table](assets/ch7-key-character-table.png)
*Key-character substitution table — multiple alphabets selected by keyword*

![Alphabet grid for substitution](assets/ch7-alphabet-grid.png)
*Alphabet grid showing letter mappings for the key-character system*
- [ch-3-speech-in-words](concepts/ch-3-speech-in-words.md) — spoken substitution (transmutation)
- [polybius-cipher](entities/polybius-cipher.md) — the coordinate-based cipher from Chapter 20
- [porta-cipher-disk](concepts/porta-cipher-disk.md) — the wheel character mentioned as further refinement
- [atbash](concepts/atbash.md) — the Athbash cipher in detail
