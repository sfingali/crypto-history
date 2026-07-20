---
title: "Porta vs Wilkins on Cipher Methodology: Mechanic vs Information Theorist"
created: 2026-07-20
updated: 2026-07-20
type: comparison
tags: [comparison, porta, wilkins, cryptography, cipher-disk, frequency-analysis, steganography, binary-alphabet, 16th-century, 17th-century]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Porta vs Wilkins on Cipher Methodology: Mechanic vs Information Theorist

**Giambattista della Porta** (1535–1615) was the most cited cryptographic authority in [[mercury-wilkins|*Mercury*]], and **John Wilkins** (1614–1672) was his most thorough reader. But their approaches to cryptography differ dramatically. Porta was a practitioner and inventor — a man who built cipher disks and tested secret inks in his Neapolitan laboratory. Wilkins was a systematiser and educator — a man who read everything, organised everything, and explained everything, including the things Porta himself admitted were beyond explanation.

## Dimensions of Comparison

| Dimension | Giambattista della Porta | John Wilkins |
|-----------|--------------------------|--------------|
| **Primary work** | *De Furtivis Literarum Notis* (1563) — "On the Secret Marks of Letters" | *Mercury: or the Secret and Swift Messenger* (1641) |
| **Scope** | Narrower: substitution ciphers, cipher disk, frequency analysis, secret inks, some optical signalling | Broader: all of the above plus gesture systems, universal characters, shorthand, musical ciphers, telegraphy, steganography, and the moral defence of cryptography |
| **Central metaphor** | The **machine**: the cipher disk as a physical device that performs encryption by mechanical rotation | The **system**: ciphers as instances of general principles of information encoding across any medium |
| **Key practical contribution** | The **cipher disk**: concentric rotating alphabets for rapid substitution | The **binary alphabet**: reducing all communication to two symbols, applicable to torches, bells, fingers — any binary medium |
| **Frequency analysis** | Provided systematic rules for breaking substitution ciphers by letter frequency — the first published cryptanalytic method | Expands Porta's rules with more thorough instruction, connecting frequency analysis to the specific properties of different languages |
| **Secret inks** | Extensive catalogue in *Magia Naturalis* (1558/1589): putrified willow, distilled glow-worms, salt armoniac, alum, onion juice, lemon juice | Cites Porta's catalogue faithfully but adds his own systematisation by category (heat-revealed, water-revealed, light-revealed, etc.) |
| **Steganography** | Mentioned but secondary to cryptographic substitution | **Central** — the entire [[ch-4-secret-conveyances|Chapter 4]] is devoted to physical concealment, and "freedom from suspicion" is a recurring theme |
| **Admission of limits** | Confessed some ciphers are unbreakable: *"Multa esse posse furtiva scripta, quae se interpretaturum quenquam polliceri, furorem et delirium plane existimarem"* — "I would consider it madness and delirium for anyone to promise he could interpret them" | Cites this confession approvingly and uses it to argue against Scaliger's dismissal of cryptography as a needless art |
| **Relationship to magic** | Ambiguous — his *Magia Naturalis* straddles the line between experimental science and Renaissance occultism; his Academy was suppressed by the Inquisition | Clear demarcation: genuine cryptography vs "magical, or fabulous" claims, relegated to [[ch-19-fabulous-magical|Chapter 19]] for debunking |
| **Tone and audience** | Renaissance virtuoso writing for fellow experimenters and patrons | Protestant clergyman writing a systematic textbook for "statesmen and soldiers" and fellow scholars |
| **Historical self-awareness** | Claims primacy as a discoverer | Self-consciously builds on predecessors, citing Porta more often than any other authority |

## Mechanical Focus vs Information-Theoretic Insight

Porta's cipher disk is a **mechanical solution** to a cryptographic problem. Set the inner disk to a pre-arranged position (the key) and read plaintext on the outer ring, ciphertext on the inner. It's elegant, practical, and you can hold it in your hand. It is the ancestor of the Confederate cipher disk, the Enigma machine, and every mechanical encryption device that followed.

But the cipher disk solves only **one** problem: substitution. It doesn't address transposition, steganography, signalling, or language-independent communication — all of which Wilkins covers.

Wilkins's great insight is more abstract: **any alphabet can be reduced to two symbols** through systematic transposition through five places. This is not a machine — it's a **principle**. It means that any medium with at least two distinguishable states (torch raised/lowered, bell/trumpet, finger extended/curled, Roman type/Italic) can encode any message. This is the insight that connects [[ch-9-barbarous-words|Chapter 9]] (fewer-letter ciphers) to [[ch-20-polybius-torch-cipher|Chapter 20]] (the Polybius torch telegraph) to [[ch-14-signs-gestures|Chapter 14]] (finger-signing).

Porta gave the world a better lock. Wilkins gave the world a theory of locks.

## Practitioner vs Educator

Porta was an experimenter. He tested secret inks in his laboratory. He founded the **Accademia Secretorum Naturae** — possibly the first scientific society — where members presented experimental findings. His accounts of secret inks carry the authority of personal trial: "as Porta affirms from his own experience."

Wilkins was an educator. His goal in *Mercury* is not to invent new ciphers (though he does offer his own systems) but to **teach** the reader everything known about secret communication. His method is the textbook writer's method: classify, explain, compare, provide examples. Where Porta says "here is a thing I discovered," Wilkins says "here is everything known about this class of things, and here is how they relate."

This difference shows in their treatment of frequency analysis. Porta gives you the rules. Wilkins gives you the rules *and* explains why they work *and* connects them to the specific properties of English, Latin, and other languages *and* warns you about the limitations. Porta wrote for fellow adepts; Wilkins wrote for anyone who could read.

## What Wilkins Adds That Porta Didn't Cover

The comprehensive scope of *Mercury* reveals what was missing from Porta's narrower focus:

### 1. Steganography as a Systematic Art

Porta mentions physical concealment methods (the Navarre story is a vivid example), but Wilkins elevates "freedom from suspicion" to a governing principle. [[ch-4-secret-conveyances|Chapter 4]] catalogues every classical trick — the hare's belly, the wax tablet, the scalp tattoo, the swallowed box — as evidence that cryptography proper renders such bodily extremes unnecessary. The argument is: learn ciphers and you won't need to swallow your messages.

### 2. The Binary Alphabet

Porta's cipher disk rotates one alphabet against another. Wilkins's binary alphabet (via Bacon's biliteral principle) reduces the alphabet to **two symbols**. This is a fundamentally different kind of insight — not mechanical but **information-theoretic**. It anticipates the logic of digital encoding.

### 3. Gesture and Sign Systems

Porta says nothing about [[ch-14-signs-gestures|finger-signing, gestural communication, or the deaf]]. Wilkins devotes an entire chapter to *arthrologia* and *dactylologia*, citing [[bede|the Venerable Bede]] and Pierius Valerianus as authorities, and developing his own finger alphabet. This expansion from written ciphers to **embodied communication** is entirely Wilkins's contribution.

### 4. The Universal Character

Porta shows no interest in language-independent writing. Wilkins's [[ch-13-universal-character|Chapter 13]] — the seed of his later *Essay* — proposes a system of characters that represent "things and notions" directly, legible to all nations regardless of spoken language. This is a vision that goes far beyond cryptography into linguistics and philosophy.

### 5. The Moral Framework

Porta simply presents his methods. Wilkins frames *Mercury* with a theological argument (the [[conclusion-moral-defense|Conclusion]]) that secret communication is not inherently suspicious but is a legitimate tool when used for just ends. He also carefully separates genuine technique from magical imposture — a demarcation Porta, whose *Magia Naturalis* was investigated by the Inquisition, could never fully achieve.

### 6. Speed as a Coordinate Axis

Wilkins's subtitle — *the Secret **and Swift** Messenger* — introduces speed as a dimension of communication equal to secrecy. Porta's focus is entirely on hiding meaning. Wilkins considers how to transmit messages quickly across distance (torches, bells, carrier pigeons), treating secrecy and swiftness as complementary goals.

## The Navarre Story: Where They Meet

One story illustrates the relationship perfectly. Porta recounts the siege of Navarre, where a man swallowed a box containing a letter, walked through enemy lines disguised as a deserter, and later recovered the box to deliver his message. Wilkins retells this in [[ch-4-secret-conveyances|Chapter 4]], pairing it with [[josephus|Josephus's]] story of Jews swallowing gold at the siege of Jerusalem.

Both stories serve the same rhetorical purpose in Wilkins's hands: they demonstrate the **desperation of the pre-cryptographic world**. People went to these extremes "for want of skill in this subject that is here discoursed of." Wilkins treats Porta's story not as a recommended method but as evidence of the need for better methods — the methods Wilkins himself provides.

## Synthesis and Verdict

Porta was the greater inventor. His cipher disk, his frequency analysis rules, his secret ink formulations — these are genuine contributions to cryptographic technology. Wilkins's *Mercury* would be impossible without Porta's *De Furtivis*.

But Wilkins was the greater **thinker** about cryptography. He saw connections Porta didn't: between cipher systems and signalling systems, between secrecy and speed, between cryptography and universal language, between the biliteral cipher and the torch telegraph. His work is not only more comprehensive but more **integrated** — a unified theory of secret communication.

If Porta is the master locksmith, Wilkins is the first professor of lock-picking. One built better tools; the other built the discipline.

## Cross-References

- [[porta-baptista]] — full entity page
- [[john-wilkins]] — full entity page
- [[mercury-wilkins]] — the book
- [[porta-cipher-disk]] — technical details of the cipher disk
- [[ch-7-equal-letters-powers]] — the wheel character in *Mercury*
- [[ch-9-barbarous-words]] — the binary alphabet principle
- [[ch-4-secret-conveyances]] — the Navarre story in context
- [[ch-5-materials]] — secret inks
- [[ch-11-invented-characters]] — frequency analysis
- [[ch-20-polybius-torch-cipher]] — the binary principle in telegraphy
- [[ch-19-fabulous-magical]] — demarcating science from magic
- [[trithemius]] — the third pre-Wilkins authority
