---
title: "Chapter 6: Secret Writing by Changing the Places of Letters — Transposition Ciphers"
created: 2026-07-20
updated: 2026-07-20
type: concept
tags: [cryptography, wilkins, mercury, transposition, cipher, anagram]
book: mercury
chapter: 6
sources: [raw/mercury-1802.txt]
confidence: high
---

# Chapter 6: Secret Writing by Changing Places

This chapter begins the core of **Cryptographia** — secret writing — by addressing the first method of obscuring meaning with the common alphabet: **transposition** (rearranging letters without altering their values).

## The Framework

> "That secrecy which does consist in the form of writing, is when the words or letters are so framed by compact, that they are not of ordinary signification."

Wilkins quotes St. Augustine approving human inventions like shorthand (*notae*) and distinguishes them from magical practices. Then he structures the field:

Secret writing can use:
1. **Common letters** — Chapters 6-10
2. **Invented notes and characters** — Chapters 11-13

Both are divisible into methods using:
1. **Equal** number of signs as natural writing
2. **More** signs
3. **Fewer** signs

Secret writing with **equal letters** works by changing either:
1. Their **places** — this chapter
2. Their **powers** — Chapter 7

## Transposition of Lines

Wilkins describes writing that reverses direction at each line — like boustrophedon, "as in the eastern languages; or from the top to the bottom, and so upward again, as is commonly related to be usual amongst the inhabitants of Taprobana in the South Sea, with those in China and Japan."

He provides an example where reading begins at the first letter towards the right hand, goes down, then up again. Decoded, it reads:

> *"The pestilence doth still increase amongst us; we shall not be able to hold out the siege without fresh and speedy supply."*

## Transposition of Letters

A man may obscure sense "by transposing each letter, according to some unusual order. As, suppose the first letter should be at the latter end of the line, the second at the beginning, or the like."

## Transposition of Both Lines and Letters Together

Wilkins provides a worked example where letters are split across two lines:

> *Teoliraelmsfnis esplvo weutel*
> *hsudesralo tai hd,upysre msyid*

Reconstructed: *"The soldiers are almost famished; supply us, or we must yield."*

### Four-Line Transposition

The method can be further obscured by spreading across four lines with a **discontinuous order**:

- First letter: beginning of line 1
- Second: beginning of line 4
- Third: end of line 1
- Fourth: end of line 4
- Fifth: beginning of line 2
- Sixth: beginning of line 3
- Seventh: end of line 2
- Eighth: end of line 3

His example ciphertext:

> *Wmrpitahhscteinpke*
> *h a thfono ihkftoenil*
> *a noerroc gt tthmnvrl*
> *e a uomhte inlenett es*

Decodes to: *"We shall make an irruption upon the enemy from the north at ten of the clock this night."*

## Increasing Obscurity

The method "will yet seem more obscure, if each line be severed into such words as may seem barbarous" — breaking the ciphertext into meaningless word-like chunks.

## Limits and Possibilities

> "All these kinds may be varied unto divers other more intricate transpositions, according as a man's fancy or occasion shall lead him."

Wilkins notes that these are only the most "remarkable" examples "either for their antiquity or usefulness." The variations are limitless.

## Key Quotes

> "This way of secret writing may be contrived, either 1. By the common letters. 2. Or by some invented notes and characters instead of them."

> "All these kinds may be varied unto divers other more intricate transpositions, according as a man's fancy or occasion shall lead him."

## Connections

- [ch-7-equal-letters-powers](concepts/ch-7-equal-letters-powers.md) — the second method of equal-letter secrecy (substitution)
- [ch-8-more-letters](concepts/ch-8-more-letters.md) — writing with more letters than needed
- [ch-3-speech-in-words](concepts/ch-3-speech-in-words.md) — spoken transposition (inversion, the oral counterpart)
- [ch-11-invented-characters](concepts/ch-11-invented-characters.md) — the next class (invented rather than common characters)
