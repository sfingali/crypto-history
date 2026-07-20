---
title: "Chapter 20: Natural and True Methods — Fires, Smokes, and the Polybius Torch Cipher"
created: 2026-07-20
updated: 2026-07-20
type: concept
tags: [cryptography, wilkins, mercury, polybius, torch-cipher, signalling, beacons]
book: mercury
chapter: 20
sources: [raw/mercury-1802.txt]
confidence: high
---

# Chapter 20: Natural and True Methods — Fires and Smokes

The final and most practical chapter. Having dispensed with fables and magic, Wilkins presents **three real systems** for communication by fire and smoke — including the Polybius torch cipher, which remains one of the most elegant encoding systems ever devised.

## The Antiquity of Fire Signalling

Fire signals are ancient:

- **Sinon** (Trojan War): "The first invention of them is commonly ascribed to Sinon" — this was the signal on which the wooden horse was unlocked (*flammas cum regia puppis extulerat*)
- **Medea**: Diodorus Siculus claims she used them in her conspiracy with Jason
- **Herodotus**: records their use in the Greek war against Xerxes
- **Thucydides**: attests to them at Salamis and the siege of Corcyra
- **Scipio at Numantia** (Appian): divided his camp into companies, each commanded: "if the enemy did charge, in the day-time they should signify it by holding up a red cloth, in the night by fires"

The Greeks called these fire-signals *phryctoi* or *pyrsoi*. Originally they answered only a specific pre-agreed question (e.g., "are allies coming or enemies?"). The torch was shaken for enemies, held still for friends.

## System 1: Polybius's Ten-Torch Cipher

This is the system's crown jewel. Wilkins describes it as "more exact."

### The Setup

The alphabet is divided into **five tablets or columns**:

| | I | II | III | IV | V |
|---|---|---|---|---|---|
| **1** | a | f | l | q | v |
| **2** | b | g | m | r | w |
| **3** | c | h | n | s | x |
| **4** | d | i | o | t | y |
| **5** | e | k | p | u | z |

Ten torches: **five on the right hand, five on the left**.

### Encoding

- Torches raised on the **right** hand = the column number
- Torches raised on the **left** hand = the row number

**Example: signaling "HASTEN"**

```
H: 2 right, 3 left  → second column, third letter = H
A: 1 right, 1 left  → first column, first letter = A
S: 3 right, 4 left  → third column, fourth letter = S
T: 4 right, 1 left  → fourth column, first letter = T
E: 1 right, 5 left  → first column, fifth letter = E
N: 3 right, 3 left  → third column, third letter = N
```

This is the **Polybius square**, still taught in cryptography courses today. Each letter requires one simultaneous display of two torch-counts. The system is fast, unambiguous, and needs no complex encoding.

## System 2: Fortius's Three-Torch System

Joachimus Fortius proposed an alternative requiring only three torches:

- **1 torch alone** = letters A–H (shown 1–8 times)
- **2 torches together** = letters I–Q (shown 1–8 times)
- **All 3 torches** = letters R–Z (shown 1–8 times)

**Example: signaling "FAMINE"**
- F: 1 torch × 6
- A: 1 torch × 1
- M: 2 torches × 4
- I: 2 torches × 1
- N: 2 torches × 5
- E: 1 torch × 5

Wilkins notes this requires "some intermission betwixt the expression of several letters, because otherwise there must needs be a great confusion." It's slower and "much more tedious and inconvenient than the former invention out of Polybius."

## System 3: Two-Torch by Motion

The fastest of all — described in the 1694 PDF with detailed diagrams:

**Principles:**
- The two torches are placed about four cubits apart
- Letters are signified by **the position and motion** of the torches, not by count
- After each signal, torches are hidden so letters can be distinguished

**The code (from the 1694 edition):**

Single torch:
- Appearing still = A
- Lifted up = E
- Depressed = I
- Inclined right = O
- Inclined left = V

Two torches:
- Both elevated = B
- Both depressed = C
- Both inclined right = D
- Both inclined left = F
- Right torch elevated = G
- Right torch depressed = H
- Right inclined right = K
- Right inclined left = L
- Left torch elevated = M
- Left depressed = N
- Left inclined right = P
- Left inclined left = Q
- Right toward left + left toward right = R
- Right inclined left + left elevated = S
- Right inclined left + left depressed = T
- Left inclined right + right elevated = W
- Left inclined right + right depressed = X
- Right inclined right + left elevated = Y
- Right inclined right + left depressed = Z

This is **semeaphore before semaphore** — a visual signalling system encoding the entire alphabet through the physical positions of two objects, decades before the Chappe optical telegraph.

## Smoke by Day

Smoke signals follow the same principles but require "tunnels provided, for the orderly inclosing and conveying up the smoke." The Chinese are said to use this system to inspect arriving merchants — asking "whence they come, what commodities they bring, and of what number they are" — the watch informing the king by smoke by day and fire by night, who "as speedily returns them his pleasure."

## Range and Multiplication

The system's range depends on line-of-sight. Like beacons (already used across England for invasion warnings), signals can be **multiplied** — handed from station to station — covering "many scores of miles." Telescopes (Galileo's perspective) can extend this further.

## Why This Matters

> "The practice of all these secret and swift messages, may perhaps seem very difficult at the first; but so does also the art of writing and reading to an unlettered man. Custom and experience will make the one as facile and ready as the other."

Wilkins then explicitly connects these methods back to the book's origin: Godwin's *Nuntius Inanimatus*. Quoting the Latin passages from Godwin about sound and sight signals, Wilkins shows that the cryptic promises in that pamphlet — which "at the first perusal, did rather raise my wonder than belief" — are exactly these methods. ^[1802:8800-8950]

## Diagrams in the Original

The 1694 edition contains woodcut diagrams of the torch configurations:

![ch20-polybius-grid.png](assets/ch20-polybius-grid.png)
*Polybius 5×5 grid — columns I–V, rows 1–5*

![ch20-two-torch-code.png](assets/ch20-two-torch-code.png)
*Two-torch position code — all 24 letters signalled by torch position and motion*

These are among the earliest printed illustrations of a cryptographic signalling system.
