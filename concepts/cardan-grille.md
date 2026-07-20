---
title: Cardan Grille
created: 2026-07-20
updated: 2026-07-20
type: concept
tags: [cryptography, steganography, cardano, wilkins, mercury]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Cardan Grille

A steganographic method attributed to **Girolamo Cardano** (1501–1576), described in his *De Subtilitate* (1550). A sheet of paper with strategically cut holes is placed over an innocent-looking letter; only the letters visible through the holes form the secret message. The recipient, possessing an identical grille, extracts the hidden text by the same method.

Wilkins references this technique in [Chapter 8](concepts/ch-8-more-letters.md) of *Mercury* as part of his survey of methods for concealing a message within a larger, innocent text. The grille is notable because — unlike ciphers that produce obviously scrambled output — it leaves the carrier text looking perfectly normal, satisfying Wilkins's second condition for secrecy (freedom from suspicion).

The method is a forerunner of modern visual cryptography and share-based secret splitting.

## Connections

- [ch-8-more-letters](concepts/ch-8-more-letters.md) — the chapter where Wilkins describes it
- [porta-baptista](entities/porta-baptista.md) — Cardano's younger contemporary, who developed his own cipher systems
