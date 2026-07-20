---
title: "Chapter 11: Invented Characters — Points, Lines, Figures, and Frequency Analysis"
created: 2026-07-20
updated: 2026-07-20
type: concept
tags: [cryptography, wilkins, mercury, frequency-analysis, invented-characters, geometrical-cipher, steganography]
book: mercury
chapter: 11
sources: [raw/mercury-1802.txt]
confidence: high
---

# Chapter 11: Invented Characters — Points, Lines, Figures, and Frequency Analysis

Wilkins transitions from ciphers using common letters to those using **invented characters** — custom symbols, geometrical marks, and pictorial ciphers. This chapter also contains one of the earliest English-language descriptions of **frequency analysis** for breaking ciphers.

## Three Kinds of Invented Characters

> "The difference of characters, whereby several languages are expressed, is part of the second general curse in the confusion of tongues."

Wilkins classifies invented characters by what they represent:

1. **Letters** — arbitrary symbols that stand for alphabet letters
2. **Words** — characters that represent entire words (shorthand)
3. **Things and notions** — symbols that represent concepts directly (universal characters)

This chapter focuses on the first kind.

## Invented Alphabets

### The Hebrew Character Theory

> "Some learned men refer the Hebrew character that is now in use; affirming, that Ezra first invented it, thereby the better to conceal the secrets of their law, and that they might not have so much as their manner of writing common with the Samaritans and other schismatics."

The square Hebrew script, on this theory, was itself a cryptography measure.

### Ease of Creation

> "It were but needless to set down any particulars of this kind, since it is so easy for any ordinary man to invent or vary them at pleasure."

## Frequency Analysis: How to Break These Ciphers

This is among the most technically significant passages in the book — an early articulation of systematic cryptanalysis:

### Step 1: Identify Vowels

> "Endeavour to distinguish betwixt the vowels and consonants. The vowels may be known by their frequency, there being no word without some of them. If there be any single character in English, it must be one of these three vowels, A, I, O."

### Step 2: Letter Frequency

> "Search after the several powers of the letters: for the understanding of this, you must mark which of them are most common, and which more seldom used. (This the printers in any language can easily inform you of, who do accordingly provide their sets of letters.)"

This is the **frequency analysis principle**: printers knew the relative frequency of letters because they needed to stock type accordingly. Wilkins advises identifying which letters can be doubled (H, Q, X, Y cannot) and which cannot.

### Step 3: Positional Analysis

Create tables for "the number of vowels or consonants in the beginning, middle, or end of words" to "readily guess at any word, from the number and nature of the letters that make it":
- Words consisting only of vowels
- One vowel + one consonant combinations (vowel first: *am, an, as, if, in, is, it, of, on, or, us*; consonant first: *be, he, me, by, dy, fly, my, thy, do, to, so*)

"These tables must be various, according to the difference of languages."

Wilkins acknowledges: "There are divers the like rules to be observed, which are too tedious to recite; you may see them largely handled by Baptista Porta, and Gustavus Selenus."

### Countermeasures: How to Defeat Frequency Analysis

> "The common rules of unfolding being once known, a man may the better tell how to delude them."

1. **Omit rare letters** (H, K, Q, X, Y) and use their characters to **represent vowels**, so vowels get double representation and are harder to identify
2. **Write continuously** — no spaces between words
3. **False word breaks** — insert spaces at wrong positions
4. **Insert nulls** — non-significant characters that don't map to any letter

### Layers of Security

> "These characters are besides liable to all those other ways whereby the common letters may be obscured, whether by changing their places, or their powers."

## The Grand Inconvenience: Suspicion

> "It is the grand inconvenience of all these ways of secrecy by invented characters, that they are not without suspicion."

A page of strange symbols is inherently suspicious — violating the second condition of good secrecy.

## Geometrical Ciphers: Unsuspected Messages

To remedy suspicion, Wilkins presents ciphers that hide in plain sight as mathematical diagrams:

### Points Alone

A line of dots at different vertical positions, where each position maps to a letter on a reference card.

### Lines Alone

Similar — line segments of varying slopes encoding letters.

### Mathematical Figures

Angles, triangles, and other geometric shapes where "the points, the ends of the lines, and the angles of the figures, do each of them, by their different situations, express a several letter." Wilkins provides a diagram of a complex geometric cipher where the figures encode:

> *"There is no safety but by flight."*

### The Reference Card

A thin narrow plate with the alphabet at equal distances serves as the directory. The paper is "secretly divided into equal parts, according to the breadth of the plate" — applying the plate reveals the letters.

### Triangular Variant

The alphabet can also be arranged in a triangular form with the middle cut out.

### Landscape Steganography

> "It is easy to apprehend by these particulars, how a man may contrive any private saying in the form of a landscape, or other picture."

This is the highest art: a secret message hidden in a drawing of trees, hills, and water, where no one would suspect anything but art.

## Key Quotes

> "Endeavour to distinguish betwixt the vowels and consonants. The vowels may be known by their frequency, there being no word without some of them."

> "The common rules of unfolding being once known, a man may the better tell how to delude them."

> "It is the grand inconvenience of all these ways of secrecy by invented characters, that they are not without suspicion."

## Connections

- [ch-6-transposition](concepts/ch-6-transposition.md) — transposition applied to invented characters
- [ch-7-equal-letters-powers](concepts/ch-7-equal-letters-powers.md) — substitution applied to invented characters
- [ch-12-shorthand](concepts/ch-12-shorthand.md) — characters expressing words (stenography)
- [ch-13-universal-character](concepts/ch-13-universal-character.md) — characters expressing things and notions

## Diagrams in the Original

Wilkins's geometrical ciphers are best appreciated through the 1694 woodcuts:

![ch11-points-cipher.png](assets/ch11-points-cipher.png)
*Points-alone cipher — dots at varying heights encode letters*

![ch11-lines-cipher.png](assets/ch11-lines-cipher.png)
*Lines-alone cipher — line segments of varying slope*

![ch11-mathematical-figures.png](assets/ch11-mathematical-figures.png)
*Mathematical figures — triangles and circles encoding text as geometry* ^[1802:6416-6550]
- [frequency-analysis](concepts/frequency-analysis.md) — the method in detail
- [porta-baptista](entities/porta-baptista.md) — Porta's detailed treatment of frequency analysis
