---
title: Bacon's Biliteral Cipher
created: 2026-07-20
updated: 2026-07-20
type: concept
tags: [cryptography, bacon, cipher, binary, wilkins, mercury]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Bacon's Biliteral Cipher

Francis Bacon's biliteral cipher, described in his *De Augmentis Scientiarum* (1623), encodes any letter of the alphabet using only two symbols (A and B) in groups of five — producing 2⁵ = 32 combinations, more than enough for 24 letters. This is directly referenced by Wilkins in [Chapter 9](concepts/ch-9-barbarous-words.md) as the theoretical underpinning of the binary alphabet system he uses throughout *Mercury*.

The cipher works by assigning each letter a 5-bit binary code: A = aaaaa, B = aaaab, C = aaaba, and so on. The inscription can then be hidden in anything that has two discriminable states — two fonts, two colours of thread, even the stems of plants in a garden.

This is the **first binary encoding of the alphabet in Western cryptography** and a direct ancestor of modern digital encoding. Bacon's genius was recognising that *any medium* with two distinguishable states can carry text — a principle Wilkins exploits for his bell, torch, and cannon systems in [Chapters 17](concepts/ch-17-joining-secrecy-swiftness-sound.md) and [20](concepts/ch-20-polybius-torch-cipher.md).

## Connections

- [bacon-francis](entities/bacon-francis.md) — Bacon's biography and full works
- [ch-9-barbarous-words](concepts/ch-9-barbarous-words.md) — Wilkins's full treatment of the binary alphabet
- [polybius-cipher](entities/polybius-cipher.md) — another coordinate-based encoding system
