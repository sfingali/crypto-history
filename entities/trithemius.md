---
title: Johannes Trithemius
created: 2026-07-20
updated: 2026-07-20
type: entity
tags: [trithemius, 16th-century, cryptography, steganography, medieval, magic, wilkins]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Johannes Trithemius (1462–1516)

**Johannes Trithemius** (born Johann Heidenberg) was a German Benedictine abbot, scholar, and cryptographer whose works *Steganographia* and *Polygraphia* are among the most controversial and influential texts in the history of secret communication. [[john-wilkins|John Wilkins]], in [[mercury-wilkins|*Mercury*]], treats Trithemius with respect but also with caution — his reputation for magic required careful handling.

## Life

Born in Trittenheim on the Moselle in 1462, Trithemius entered the Benedictine abbey of Sponheim in 1482 and became its abbot the following year, aged only 21. He transformed Sponheim's library from a few dozen volumes into one of the finest in Germany — over 2,000 manuscripts and printed books — and made the abbey a centre of humanist learning.

He wrote extensively on history, theology, demonology, and cryptography. His historical works include *De Viris Illustribus Germaniae* (1495), an early national bibliography. But it is his cryptographic writings that ensured his long, strange fame.

## *Steganographia* (c. 1499, published 1606)

*Steganographia* ("Secret Writing") is the work that made Trithemius notorious. Written around 1499 but not published until 1606 (ninety years after his death), it purported to teach methods of communicating secretly over distances — but it did so by invoking **spirits**.

The book is divided into three books:

- **Book I**: Describes how to summon spirits to carry messages. Each spirit is associated with a particular planet, hour, and angelic hierarchy.
- **Book II**: Contains "conjurations" addressed to spirits called by name — "Pamerfiel," "Padiel," "Camuel," and others — for sending messages instantly to any part of the world.
- **Book III**: The most occult section, involving elaborate rituals with planetary angels.

The entire work is written in a strange, incantatory style that reads as genuine necromancy. But this was almost certainly a **disguise** — a "cover cipher" designed to scare off the vulgar and protect the book's real content: cryptographic tables and encoding methods hidden beneath the magical veneer.

### The Burning of the Manuscript by Frederick II

Wilkins records that **Frederick II, Prince Palatine**, acting on the advice of **Junius** (a Protestant theologian), **ordered the original manuscript of *Steganographia* to be burned**. The passage that most alarmed them described "the three saturnine angels, and certain images, by which, in the space of twenty-four hours, a man may be informed of news from any part of the world."

Selenus (Gustavus Selenus, author of *Cryptomenytices et Cryptographiae*, 1624) later declared this burning **unjust** — the book was cryptography, not magic. Wilkins agrees, suggesting in Chapter 20 of *Mercury* that Trithemius may have been describing a network of **signal stations** (beacon chains), with the "angels" serving as metaphors for the intermediate relay points.

## *Polygraphia* (1518)

Published posthumously, *Polygraphia* ("Many Writings") is Trithemius's openly cryptographic work — no spirits, no demons. It contains:

- **The *tabula recta***: a square of alphabets — the ancestor of the Vigenère cipher. Each row begins with the next letter, producing a table of 24 × 24 letters (J and V omitted). This is the key-character system that Wilkins describes in [[ch-7-equal-letters-powers|Chapter 7]].
- **The *Ave Maria* cipher**: messages disguised as prayers
- **Code-book systems**: pre-arranged tables where each plaintext letter maps to a word; Wilkins describes this method in [[ch-8-more-letters|Chapter 8]] as "much insisted on by Trithemius, Porta, and Sylenus"

*Polygraphia* is the **first printed book on cryptography** — though *Mercury* (1641) is the first in English.

## Wilkins's Treatment in *Mercury*

Wilkins mentions Trithemius in multiple chapters, carefully negotiating the tension between admiration and orthodoxy:

### Chapter 1: Ancient and Modern Authorities
Wilkins lists Trithemius first among the modern authors on secret communication — "The Abbot Trithemius" — alongside Bibliander, Porta, Cardan, Casaubon, Walchius, Selenus, Vossius, and Hugo.

### Chapter 8: The Code-Book Cipher
"Trithemius, Porta, and Sylenus" are credited with the method where each word or form of an epistle is varied to as many differences as there are letters — the code-book approach to substitution.

### Chapter 12: Shorthand and Stenography
Trithemius claims that Cicero himself wrote a treatise on shorthand, later augmented by St. Cyprian. He also reports finding in an old library a copy of a psalter written in Tironian notes, mistakenly titled *Psalterium in Lingua Armenica*.

### Chapter 15: The Burned Manuscript
Wilkins provides the most detailed account: Trithemius "does pretend to handle the forms of conjuration, calling each kind of character by the name of spirits, thereby to deter the vulgar from searching into his works." The three saturnine angels passage went too far, and Frederick II burned the original.

### Chapter 20: Rehabilitation
Wilkins's most interesting move: he suggests that Trithemius's "spirits" may have been code for **signal relays** — human messengers stationed at intervals, like a chain of beacons. If so, "that author might then in one respect, be freed from the aspersion of diabolical magic."

## The Cipher Beneath

The *Steganographia* was conclusively deciphered in the 20th century: the spirit names were cryptographic keys, and the incantations concealed ciphertext revealing simple substitution and transposition systems. Trithemius had, in effect, written a cryptography textbook disguised as a grimoire — the ultimate steganographic work.

This makes him perhaps the only author in history whose cryptography was so good it got his book burned.

## Reputation for Magic

Trithemius's reputation for magic was not undeserved: he also wrote *De Septem Secundeis* (on the seven planetary intelligences governing history), engaged in the angelic magic of the Renaissance Hermetic tradition, and was accused by contemporaries of necromancy. His humanist learning — vast but sometimes credulous — made it impossible for later readers to cleanly separate the cryptographer from the occultist.

Wilkins's gentle but persistent defence of Trithemius reflects a broader 17th-century project: reclaiming the useful content of Renaissance magic while discarding its superstitions. It is the same move that produced modern chemistry from alchemy.

## Cross-References

- [[mercury-wilkins]] — Wilkins's treatment of Trithemius
- [[ch-15-spiritual-substances]] — the burned manuscript and saturnine angels
- [[ch-8-more-letters]] — the code-book cipher
- [[ch-7-equal-letters-powers]] — the tabula recta as ancestor of key-character
- [[ch-20-polybius-torch-cipher]] — Wilkins's reinterpretation as signal relays
- [[porta-baptista]] — Porta, frequently paired with Trithemius by Wilkins
