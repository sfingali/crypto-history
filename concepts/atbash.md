---
title: The ATBASH Cipher
created: 2026-07-20
updated: 2026-07-20
type: concept
tags: [cipher, cryptography, substitution-cipher, atbash, biblical-cipher, cabala, hebrew, wilkins]
sources: [raw/mercury-1802.txt]
confidence: high
---

# The ATBASH Cipher (אתבש)

The **ATBASH cipher** (Hebrew: אתבש) is one of the oldest known substitution ciphers — a reverse-alphabet substitution where the first letter of the Hebrew alphabet is replaced with the last, the second with the second-to-last, and so on. [John Wilkins](entities/john-wilkins.md) presents it in [Chapter 7](concepts/ch-7-equal-letters-powers.md) of [*Mercury*](entities/mercury-wilkins.md) as the most significant example of Hebrew cabalistic cryptography, complete with its biblical attestations.

## The Method: Reverse-Alphabet Substitution

The name **אתבש** (ATBASH) is itself a mnemonic, formed from the first four corresponding letter pairs of the cipher:

| Position | Hebrew Letter | Name | Replaced By | Name |
|----------|--------------|------|-------------|------|
| 1 | א | Alef | ת | Tav |
| 2 | ב | Bet | ש | Shin |
| 3 | ג | Gimel | ר | Resh |
| 4 | ד | Dalet | ק | Qof |
| ... | ... | ... | ... | ... |
| 22 | ת | Tav | א | Alef |

The full mapping:
```
Plain:  א ב ג ד ה ו ז ח ט י כ ל מ נ ס ע פ צ ק ר ש ת
Cipher: ת ש ר ק צ פ ע ס נ מ ל כ י ט ח ז ו ה ד ג ב א
```

In English terms (for the Latin alphabet), the ATBASH principle would map:
```
Plain:  A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
Cipher: Z Y X W V U T S R Q P O N M L K J I H G F E D C B A
```

This is the simplest possible substitution after the Caesar shift — but its conceptual root is not Roman but Hebrew, and its earliest applications are biblical.

## Biblical Applications

Wilkins presents two famous biblical examples where the ATBASH cipher was used to conceal politically sensitive names in the Hebrew Bible:

### Sheshach → Babel (Jeremiah 51:41)

> "How is Sheshach taken!"

The name **Sheshach** (ששך) appears in Jeremiah 51:41 as a feigned name for Babylon. Applied through ATBASH:

- **ש** (Shin) → **ב** (Bet)
- **ש** (Shin) → **ב** (Bet)
- **ך** (Final Kaf) → **ל** (Lamed)

Result: **בבל** — **Babel** (Babylon). The cipher concealed a prophecy against Babylon, allowing it to circulate without immediate political consequences.

### Leb Kamai → Chasdim (Jeremiah 51:1)

> "Thus saith the LORD: Behold, I will raise up against Babylon, and against them that dwell in Leb Kamai, a destroying wind."

**Leb Kamai** (לב קמי) literally means "the heart of those who rise against me." Applied through ATBASH:

- **ל** (Lamed) → **כ** (Kaf)
- **ב** (Bet) → **ש** (Shin)

→ **כשדים** = **Chasdim** (Chaldeans)

Wilkins notes that both the **Targum** (Aramaic paraphrase) and the **Septuagint** (Greek translation) "unanimously translate it so; as if in their version of it, they had chiefly respect unto this kind of cabalism." This is a significant argument: the ancient translators, by reading "Leb Kamai" as "Chaldeans," demonstrate that they understood the ATBASH cipher and considered it the intended meaning.

### Additional Examples

Though Wilkins focuses on Sheshach and Leb Kamai, scholars have identified other possible ATBASH uses in the Hebrew Bible, including Jeremiah 25:26 and several passages in the Book of Daniel. The cipher may represent an ancient scribal practice of encoding politically dangerous names.

## Relationship to Other Cabalistic Ciphers

Wilkins presents ATBASH alongside a related Hebrew cipher, **Albam** (אלבם):

| Cipher | Principle | Name Derivation |
|--------|-----------|-----------------|
| **ATBASH** (אתבש) | First ↔ Last (alef-tav, bet-shin) | First, last, second, second-last letters |
| **Albam** (אלבם) | Halves of alphabet (first with twelfth, second with thirteenth) | First four corresponding pairs |

### Albam's Biblical Example (Isaiah 7:6)

Wilkins supplies the Albam example: Isaiah 7:6 mentions **Tabeal** (טבאל), a person whom the prophet says aspires to the crown of Judah. Decoded through Albam (each letter mapped to its partner from the opposite half of the alphabet), the name reveals **Remaliah** (רמליהו), the king of Israel — "whom he was loth more expressly to nominate."

Both ATBASH and Albam belong to the broader cabalistic category that the rabbis called ***Ziruph*** or ***combinatio*** — the systematic transposition of alphabet letters "taken one for another, after any known order."

## Wilkins's Treatment in Chapter 7

Wilkins introduces ATBASH within his discussion of substitution ciphers — "secret writing by changing the powers of letters." His treatment is notable for:

1. **Biblical authority**: He presents the cipher not as a curiosity but as attested in scripture, with the ancient translations confirming the interpretation.

2. **Religious context**: "Both these kinds of secret writing, the Jewish doctors think to be frequently used by the sacred penmen of holy writ; amongst whom, the prophet Isaiah and Jeremiah are observed to be of more especial note for their skill in cabalisms."

3. **Theoretical completeness**: He supplies both the general principle (reverse-alphabet substitution) and specific applications (Sheshach, Leb Kamai, Tabeal).

4. **Historical argument**: The fact that ancient translators understood these ciphers proves their antiquity — this is not a medieval invention but an authentic biblical practice.

## Broader Significance

ATBASH is significant in the history of cryptography as:

- One of the **earliest attested substitution ciphers** — predating Caesar by centuries
- Evidence that **cryptographic practice existed in the ancient Near East**, embedded in scribal and prophetic traditions
- A demonstration that **the Hebrew Bible contains cryptographic content** — not just plaintext revelation
- The ancestor of the entire family of **monoalphabetic substitution ciphers** that dominated Western cryptography through the Renaissance

For Wilkins, ATBASH also serves an important rhetorical purpose: it proves that cryptography is **ancient and respectable**, not a modern or suspect invention. The prophets themselves used it.

## Cross-References

- [ch-7-equal-letters-powers](concepts/ch-7-equal-letters-powers.md) — the chapter where ATBASH is explained
- [mercury-wilkins](entities/mercury-wilkins.md) — *Mercury* as first English presentation of ATBASH
- [john-wilkins](entities/john-wilkins.md) — the author
- [frequency-analysis](concepts/frequency-analysis.md) — the method for breaking substitution ciphers including ATBASH
