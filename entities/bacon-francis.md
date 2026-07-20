---
title: Francis Bacon
created: 2026-07-20
updated: 2026-07-20
type: entity
tags: [bacon, 16th-century, cryptography, biliteral-cipher, scientific-method, royal-society, wilkins]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Francis Bacon (1561–1626)

**Francis Bacon**, Viscount St Alban, was an English philosopher, statesman, and jurist whose writings on scientific method and the classification of knowledge laid the intellectual foundations for the [[royal-society|Royal Society]] and profoundly influenced [[john-wilkins|John Wilkins]]. In [[mercury-wilkins|*Mercury*]], Wilkins calls him **"our English Aristotle"** — high praise from a man who generally rejected Aristotelianism — and draws on Bacon both for his general method and his specific contributions to cryptography.

## Life

Born in 1561 to Sir Nicholas Bacon (Lord Keeper of the Great Seal) and Anne Cooke Bacon (a brilliant classicist and translator), Francis Bacon studied at Trinity College, Cambridge, and Gray's Inn. He rose through the legal and political ranks under Elizabeth I and James I, becoming Solicitor General, Attorney General, and finally Lord Chancellor in 1618. His political career collapsed in 1621 when he was convicted of accepting bribes — though some historians see him as a scapegoat for wider corruption. He died in 1626, allegedly from a chill caught while stuffing a chicken with snow to test the preservative effects of cold — a fittingly experimental death.

## "Our English Aristotle"

Wilkins's epithet for Bacon — "our learned Bacon," "our English Aristotle" — appears in several places in his writings (including *Mathematical Magick* and *Mercury*). The comparison is pointed: Aristotle had dominated natural philosophy for two millennia, but his method (deduction from first principles) had produced little new knowledge. **Bacon's method** — induction from observation, systematic experiment, collaborative inquiry — was replacing it.

In *The Advancement of Learning* (1605) and *Novum Organum* (1620), Bacon argued:

1. **Reject the "Idols"** — systematic errors of mind (Idols of the Tribe, Cave, Marketplace, Theatre) that distort perception
2. **Collect facts** — exhaustively gather observations in "histories" (natural history, experimental history)
3. **Induce general laws** — from the collected facts, derive the underlying "forms" (laws of nature)
4. **Experiment to test** — use *experimentum crucis* (crucial experiments) to decide between competing theories

This programme — empirical, inductive, anti-scholastic — became the founding methodology of the Royal Society. Wilkins's *Mercury*, with its encyclopaedic collection of cryptographic facts drawn from every available source, is a Baconian "history" of secret communication.

## Cryptography Under Grammar: *The Advancement of Learning*

In Book VI of *The Advancement of Learning* (1605), Bacon classifies the arts and sciences. Cryptography — "the art of ciphering" — falls under **Grammar**, specifically under the "organ of speech" as:

> "The virtues and defects of writing... Ciphers are commonly in letters or alphabets, but may be in words."

This classification is significant: cryptography is not a branch of magic or military science, but of **language** — a rational system of encoding and decoding meaning. This framing shapes Wilkins's approach: *Mercury* treats ciphers alongside linguistics, universal characters, and shorthand, within a unified theory of communication.

## The Biliteral Cipher

Bacon's most famous cryptographic contribution is the **biliteral cipher** — a binary encoding system described in *De Augmentis Scientiarum* (1623, the expanded Latin version of *The Advancement of Learning*).

### How It Works

The key insight: **any letter of the alphabet can be expressed as a combination of only two symbols** — *a* and *b* — in groups of five. Since 2⁵ = 32, five binary positions can represent all 24 letters (I/J and U/V conflated, as was standard).

Example (using Bacon's own mapping):
```
A = aaaaa    B = aaaab    C = aaaba    D = aaabb
E = aabaa    F = aabab    G = aabba    H = aabbb
...
```

But the real genius was in **how you hide the a's and b's**. Bacon proposed using two different **typefaces** within an innocent-looking text:

> "The highest degree of cipher is to write *omnia per omnia* — anything by anything."

A printed page using a mixture of two subtly different fonts could encode a secret message in the pattern of letterforms, while the visible text said something innocent. The "a" positions could be signalled by Roman type, the "b" positions by Italic — or by any binary distinction: uppercase/lowercase, different inks, slightly different letter heights.

### Wilkins's Treatment

Wilkins describes the biliteral cipher in Chapter 9 ("Secret Writing with Fewer Letters than the Alphabet Requires," in the 1641 edition). He presents it as an instance of the general principle that any alphabet can be reduced to two symbols by systematic transposition through five places. He connects it to the binary alphabets used in the torch telegraph of [[ch-20-polybius-torch-cipher|Chapter 20]], where two torches (or two sounds, like bell and trumpet) can encode any letter through five sequential signals.

### The Bacon-Shakespeare Controversy

The biliteral cipher is central to the **Baconian theory of Shakespeare authorship** — the claim (first advanced in the 19th century) that Bacon encoded his authorship into the First Folio using biliteral cipher patterns in the typography. While most scholars dismiss this, the cipher's existence does demonstrate Bacon's genuine cryptographic sophistication.

## Influence on Wilkins

Bacon's influence on Wilkins operates at multiple levels:

1. **Method**: *Mercury* is a Baconian "natural history" of cryptography — collecting, cataloguing, and comparing every known method before drawing conclusions.

2. **Classification**: Wilkins's taxonomy of ciphers — by materials, by form (equal letters, more letters, fewer letters), by invented characters — mirrors Bacon's drive to systematise knowledge.

3. **Binary thinking**: The biliteral cipher's reduction of all difference to two symbols prefigures both the torch telegraph (two torches) and the binary logic of modern computing.

4. **Utility**: Bacon wrote that knowledge should bear fruit in "works" — practical applications. Wilkins's *Mercury*, for all its theoretical richness, never loses sight of practical communication needs: secrecy, speed, reliability.

5. **Universal language**: Bacon speculated about a "real character" in *The Advancement of Learning* — "characters that express neither letters nor words, but things and notions." This is the direct ancestor of Wilkins's [[ch-13-universal-character|Chapter 13]] and his later [[universal-language-project|*Essay*]].

## Legacy

Bacon did not found the Royal Society (he died decades before its charter), but his vision of collaborative, experimental science, expressed in *The New Atlantis* (1627) — a fictional island where "Salomon's House" conducts organised research — directly inspired its founders. Wilkins, Boyle, and their circle explicitly saw themselves as building the institution Bacon had imagined.

## Cross-References

- [[john-wilkins]] — "our English Aristotle" in context
- [[mercury-wilkins]] — *Mercury* as Baconian natural history
- [[royal-society]] — the institution Bacon's vision inspired
- [[ch-9-barbarous-words]] — the biliteral principle in fewer-letters ciphers
- [[ch-13-universal-character]] — Bacon's "real character" speculation
- [[universal-language-project]] — Wilkins's fulfilment of Bacon's linguistic vision
