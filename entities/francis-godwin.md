---
title: Francis Godwin
created: 2026-07-20
updated: 2026-07-20
type: entity
tags: [person, author, bishop, lunar-fiction, signaling, 17th-century]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Francis Godwin (1562–1633)

**Francis Godwin** was an English bishop, historian, and author whose work *Nuntius Inanimatus* (The Inanimate Messenger, 1629) directly inspired [John Wilkins](entities/john-wilkins.md) to write [*Mercury: or the Secret and Swift Messenger*](entities/mercury-wilkins.md) — the first cryptology book in English. He is also the author of *The Man in the Moone* (published posthumously in 1638), one of the first works of science fiction.

## Life

Godwin was born in 1562 in Hannington, Northamptonshire. He studied at Christ Church, Oxford, receiving his B.A. in 1581 and M.A. in 1584. He entered the church and rose steadily through its ranks: he became sub-dean of Exeter in 1587, Bishop of Llandaff in 1601, and Bishop of Hereford in 1617 — a position he held until his death in 1633.

He was a learned antiquarian and historian; his *Catalogue of the Bishops of England* (1601) was considered a significant scholarly work.

## *Nuntius Inanimatus* (1629)

This short Latin pamphlet — whose full title translates to *The Inanimate Messenger, or a Method of Making Known One's Mind to an Absent Friend by Means not Commonly Practised* — made extraordinary promises:

- A man could communicate with a friend who was locked in "a close dungeon"
- A man could communicate into a "besieged city"
- A man could communicate with someone "a hundred miles off"

Godwin claimed there were certain ways to achieve this, but wrote with deliberate obscurity. As Wilkins notes in his preface "To the Reader," these promises "at the first perusal, did rather raise my wonder than belief" — and he would have dismissed them as "altogether fabulous" had it not been for Godwin's reputation as a bishop.

### What Godwin Actually Meant

In Chapter 20 of *Mercury*, Wilkins provides the solution to Godwin's riddle. Godwin was not describing magic but **optical and acoustic telegraphy** using fires, smoke, and sound signals. Wilkins quotes Godwin's own words to prove this:

For **sound signals**: Godwin wrote that the recipient must hear *"sounds, distinguishable by the number of things to be heard"* — and these must vary *"either in kind, or in time, together with manner and number."* This directly corresponds to the binary/ternary encoding systems Wilkins describes in Chapters 9 and 17.

For **visual signals**: Godwin wrote that if you wish to represent something to the eye of an absent friend faster than any sublunary body could travel, you need *"visible forms or ideas, increased in quantity, multiplied in number, and varied in quality, quantity, situation, or order."*

### The London-to-Bristol Example

Godwin's most striking claim: a message sent from London at noon would arrive in Bristol "before twelve of the clock that day" — meaning the signal travels faster than the difference between the two meridians. Wilkins explains that this is achievable by placing signal stations on high mountains and beacon hills, relaying the message from one to the next near-instantaneously.

## *The Man in the Moone* (1638)

Godwin's other major work was published posthumously in 1638 (though written in the 1620s). It tells the story of **Domingo Gonsales**, a Spanish adventurer who travels to the Moon in a flying chariot pulled by trained swans (called *gansas*). On the Moon, he discovers a utopian society of lunar inhabitants who are Christians, tall, and communicate through **a musical language**.

### Domingo Gonsales

Gonsales is the fictional narrator and protagonist. He flees Spain after killing a man in a duel, makes his fortune in the East Indies, and on his return voyage falls ill on the island of St. Helena. There he discovers and trains the *gansas* (large swan-like birds), eventually hitching them to an "engine" that carries him to the Moon.

> Key detail: *The Man in the Moone* was written in the first person as a travel narrative, and many early readers believed it was a genuine account — much like later reactions to *Gulliver's Travels*.

### The Lunar Language (Musical Code)

The lunar inhabitants communicate through **musical tones** rather than articulate speech. Godwin printed musical notation in the book to represent their language. In Chapter 18 of *Mercury*, Wilkins **cracked this code**:

He reproduced the musical staves and demonstrated that the notes are simply an alphabetic substitution cipher:
- The **five vowels** are represented by minims on each of the five lines of the musical staff
- The **consonants** are represented by combinations of pitch and note duration
- The letters K and Q are omitted (expressible otherwise)
- The underlying language is **Latin** — words like *Gloria Deo soli* can be constructed from the musical notes

This is among the **earliest literary examples of a cryptographic puzzle embedded in fiction**, and the earliest documented crack of one.

## Influence on Wilkins

Godwin's influence on Wilkins was profound:

1. **Direct cause of *Mercury***: Wilkins states in his preface that reading *Nuntius Inanimatus* "first occasioned this discourse." He collected all his cryptographic notes and composed *Mercury* to explain what Godwin had hinted at.

2. **Shared lunar interest**: Wilkins's first book (1638), *The Discovery of a World in the Moone*, directly engages with Godwin's *The Man in the Moone*. Wilkins treats Gonsales's voyage as a thought experiment about the habitability of other worlds.

3. **The musical code**: Wilkins's successful decryption of Godwin's lunar musical language in Chapter 18 is the climax of the "joining secrecy and swiftness" section.

4. **The flying chariot**: Godwin's swan-drawn chariot influenced Wilkins's own discussions of flying machines, discussed briefly in *Mercury* (Chapter 4) and extensively in *Mathematical Magick* (1648).

## Legacy

Godwin's *The Man in the Moone* influenced later lunar fiction including Cyrano de Bergerac's *Comical History of the States and Empires of the Moon*, and arguably the entire genre of science fiction. His cryptographic puzzles in *Nuntius Inanimatus* indirectly produced the first English-language cryptology book, placing him at the intersection of literature, science, and secret communication.

## Cross-References

- [john-wilkins](entities/john-wilkins.md) — the man who cracked his code
- [mercury-wilkins](entities/mercury-wilkins.md) — the book he inspired
- [polybius-cipher](entities/polybius-cipher.md) — the torch telegraph that explains *Nuntius Inanimatus*
- [ch-18-musical-notes](concepts/ch-18-musical-notes.md) — cracking the lunar musical code
- [ch-20-polybius-torch-cipher](concepts/ch-20-polybius-torch-cipher.md) — the true method behind Godwin's promises
