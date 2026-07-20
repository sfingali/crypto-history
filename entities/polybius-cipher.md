---
title: Polybius Cipher (Torch Telegraph)
created: 2026-07-20
updated: 2026-07-20
type: entity
tags: [cipher, cryptography, ancient-greece, polybius, torch-signals, optical-telegraph]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Polybius Cipher (The Torch Telegraph)

The **Polybius cipher** is an ancient Greek optical telegraph system described by the historian **Polybius** (c. 200–118 BCE) in Book 10 of his *Histories*, and transmitted to modernity through [John Wilkins's](entities/john-wilkins.md) detailed explanation in [*Mercury*](entities/mercury-wilkins.md), Chapter 20. It is the earliest known cryptographic grid system — a method of encoding the alphabet into coordinate pairs transmitted by torch signals.

## The Method (as described in Polybius, via Wilkins)

### The Encoding Grid

The alphabet is divided into **five tablets or columns** (a 5×5 grid):

|  | I | II | III | IV | V |
|--|---|---|----|----|---|
| **1** | a | f | l | q | x |
| **2** | b | g | m | r | y |
| **3** | c | h | n | s | z |
| **4** | d | i | o | t |   |
| **5** | e | k | p | u |   |

Each letter is identified by two numbers: the **table number** (column) and the **row position** within that table. For example:
- A = column 1, row 1
- H = column 3, row 2
- S = column 4, row 3

### The Two-Torch System

The system requires **ten torches in total**: five placed on the right hand, five on the left.

- **Right-hand torches**: Indicate column number (1–5)
- **Left-hand torches**: Indicate row number (1–5)

To signal a letter, you raise the corresponding number of torches on each side simultaneously. For example, to signal **H** (column 3, row 2):
- Raise **3 torches** on the right hand
- Raise **2 torches** on the left hand

Wilkins provides a worked example for the word **HASTEN**:

| Letter | Right (column) | Left (row) |
|--------|---------------|------------|
| H | 2 lights | 3 lights |
| A | 1 light | 1 light |
| S | 4 lights | 3 lights |
| T | 3 lights | 4 lights |
| E | 5 lights | 1 light |
| N | 3 lights | 3 lights |

After each signal, the torches must be carefully hidden and obscured so the letters can be properly distinguished.

## Alternative Torch Systems Described by Wilkins

### Joachimus Fortius's Three-Torch Method

Uses only three lights, but is slower:
- **1 torch shown alone**: Signals letters A–H (shown 1–8 times)
- **2 torches together**: Signals I–Q (shown 1–8 times)
- **3 torches together**: Signals R–Z

Requires intermission pauses between letters to avoid confusion. Wilkins considers this "much more tedious and inconvenient" than Polybius's two-hand system.

### Binary Encoding with Two Torches

Using the binary alphabet described in Chapter 9 (two symbols transposed through five places = 32 differences), two torches could express any letter in five shows — but this is slower than the coordinate grid method.

### The Two-Torch Motion System (Most Swift)

Wilkins's preferred method uses **two torches on long poles**, placed about four cubits apart. Letters are expressed by the **position and motion** of the torches:

- **One light alone**: A (stationary), E (elevated), I (depressed), O (inclined right), V (inclined left)
- **Two lights together**: B (elevated), Q (depressed), D (inclined right), F (inclined left)
- **Right torch only**: G (elevated), H (depressed), K (inclined right), L (inclined left)
- **Left torch only**: M (elevated), N (depressed), P (inclined right), Q* (inclined left)
- **Complex motions**: Crossing, combined elevation/depression for R, S, T, W, X, Y, Z

This system allows each letter to be signalled with a **single motion** — making it the fastest optical telegraph until the Chappe semaphore in 1792.

## Daytime Use: Smoke Signals

For daytime communication, the same encoding principles apply but use **smoke** instead of fire. Wilkins notes that tunnels must be provided for "orderly inclosing and conveying up the smoke."

## Range Extension

Wilkins observes that by **multiplying** these signal stations in several places — like a chain of beacons — messages can be transmitted "for many scores of miles." He cites the English beacon system for spreading warnings, and notes that Galileo's telescope (the "perspective") could help read signals at greater distances.

He also relates that in China, watch-stations used smoke by day and fire by night to inform the king about approaching merchant ships, and receive his response — "that is easily dispatched in some few hours, which could not be performed the ordinary way, without the trouble of many days."

## Connection to Godwin's *Nuntius Inanimatus*

Wilkins explicitly identifies this torch/smoke system as the **true method** behind Francis Godwin's cryptic promises in [*Nuntius Inanimatus*](entities/francis-godwin.md). He quotes Godwin's Latin: signals must be *distinguibile pro numero audiendorum* (distinguishable by the number of things to be heard) and must vary *vel genere, vel tempore, modo etiam et numero* (in kind, or time, also in manner and number).

Godwin even gave a concrete example: a message from London to Bristol, arriving "before twelve of the clock" even if sent at noon — since the signal travels faster than the difference in meridians.

## Cryptographic Significance

The Polybius cipher is:
1. The **first known cryptographic grid** — the ancestor of all coordinate-based encipherment
2. A **fractionating cipher**: it splits each letter into two components (column and row)
3. The ancestor of the **ADFGVX cipher** used by Germany in WWI
4. The basis for modern **tap codes** and **knock codes** used by prisoners of war

## Cross-References

- [mercury-wilkins](entities/mercury-wilkins.md) — Wilkins's full treatment
- [ch-20-polybius-torch-cipher](concepts/ch-20-polybius-torch-cipher.md) — Chapter 20 detailed context
- [francis-godwin](entities/francis-godwin.md) — *Nuntius Inanimatus*
- [john-wilkins](entities/john-wilkins.md) — author biography
- [history-of-cryptography](concepts/history-of-cryptography.md)
