---
title: Flavius Josephus
created: 2026-07-20
updated: 2026-07-20
type: entity
tags: [josephus, classical, jewish-history, siege-of-jerusalem, steganography, wilkins, essenes, zealots]
sources: [raw/mercury-1802.txt]
confidence: high
---

# Flavius Josephus (c. 37–c. 100 CE)

**Flavius Josephus** (born Yosef ben Matityahu) was a Jewish historian and military commander whose works — particularly *The Jewish War* (*Bellum Judaicum*) — are among the most important sources for first-century Jewish history. In [[mercury-wilkins|*Mercury*]], [[john-wilkins|John Wilkins]] references Josephus for a memorably grotesque anecdote: Jews swallowing gold at the siege of Jerusalem. But Josephus's relevance to cryptography and secret communication extends further than this single story.

## Life

Josephus was born in Jerusalem around 37 CE to a priestly family. When the First Jewish-Roman War broke out in 66 CE, he was appointed military governor of Galilee. After the fall of the fortress at Jotapata, Josephus surrendered to the Romans — famously predicting (he claimed) that the Roman commander Vespasian would become emperor. When this prophecy came true in 69 CE, Josephus was freed and became a Roman citizen, adopting the family name Flavius in honour of his patron.

He spent the rest of his life in Rome, writing histories designed to explain (and justify) the Jewish people and their war to a Roman audience. His major works:

- ***Bellum Judaicum*** (*The Jewish War*, c. 75 CE): An eyewitness account of the war, including the siege and destruction of Jerusalem in 70 CE
- ***Antiquitates Judaicae*** (*Jewish Antiquities*, c. 94 CE): A history of the Jewish people from creation to the outbreak of the war
- ***Contra Apionem*** (*Against Apion*): A defence of Judaism against Greek critics
- ***Vita*** (*Life*): An autobiography

## The Jerusalem Siege Story in Full Context

Wilkins's reference to the swallowed gold comes from *Bellum Judaicum* Book 5, which describes the Roman siege of Jerusalem in 70 CE. The context is a city in terminal crisis.

By Book 5, Jerusalem is surrounded by Titus's legions. Famine rages inside the walls. Josephus describes horrors in unsparing detail: families fighting over scraps of food, mothers eating their children, the dead left unburied in the streets. The wealthier inhabitants, who had stockpiled grain, are targeted by Zealot factions who break into houses, torture residents to reveal hidden supplies, and — critically — search for gold.

The swallowed-gold episode appears in this context. Some Jewish fugitives, attempting to escape the starving and doomed city, melted their gold into small pellets and swallowed them before crossing the Roman lines, intending to recover the treasure from their bodies later. Josephus reports that the practice was discovered — possibly by Syrian auxiliaries serving with the Romans, who noticed gold in the excrement of captured fugitives. Once the secret was known, Roman soldiers began **disembowelling captives** on the spot to search for swallowed treasure.

Josephus reports this with grim resignation. The act of swallowing gold was a desperate survival strategy — take your wealth with you in the only way possible when strip-searched at enemy checkpoints. The Roman response — mass disembowelment of prisoners — was the predictable result of a secret discovered. The story is, in essence, a **steganographic failure**: the concealment method worked only until the enemy learned of it.

## Wilkins's Use of Josephus

### The Swallowed Gold (Chapter 4)

In [[ch-4-secret-conveyances|Chapter 4]] of *Mercury*, Wilkins catalogues every known method of physically concealing a written message. After describing methods involving animal carcasses, wax tablets, and scalp tattoos, he mentions the Josephus story:

> "Some of the fugitive Jews at the siege of Jerusalem did swallow down their gold in little bullets, that afterwards amongst other excrements they might recover it again."

The story is not about secret communication — it is about secret **transportation** of wealth. But Wilkins immediately connects it to his cryptographic concerns:

> "Now if a man had but his faculty, who could write Homer's Iliads in a nut-shell; it were an easy matter for him, by this trick of the Jews, securely to convey a whole pacquet of letters."

The logic is characteristically Wilkinsian: if people went to such extreme lengths for *gold* "for want of skill" in better methods, imagine what they could do with proper cryptological knowledge. The swallowed-gold story is evidence, in Wilkins's framing, of the desperation caused by the **absence of systematic cryptographic technique**. The moral is: learn ciphers and you won't need to swallow your messages — or have your belly cut open by those looking for them.

### The Jotapata Messengers (Chapter 4)

Immediately before the gold-swallowing passage, Wilkins cites Josephus for a second anecdote:

> "Some messengers have been sent away in coffins as being dead: some others in the disguise of brute creatures, as those whom Josephus mentions in the siege of Jotapata, who crept out of the city by night like dogs."

The footnote in the 1802 text confirms the source: *De Bello Judaic. l. 3. c. 8*. During the siege of Jotapata (67 CE), when Josephus himself was the defending commander, he sent messengers who crawled on all fours past Roman sentries under cover of darkness. The animal disguise — "like dogs" — is a form of physical steganography: concealment through behaviour rather than cryptography.

Both stories serve the same rhetorical purpose in *Mercury*: they are evidence of the **ingenuity born of desperation** when normal communication is impossible — the exact problem that cryptography, Wilkins argues, can solve without bodily risk.

## Josephus's Broader Relevance to Cryptography

Josephus is not a cryptographer. But his histories contain material directly relevant to the history of secret communication:

### The Essenes' Secret Books

In *Bellum Judaicum* Book 2, Josephus describes the Essenes — the Jewish sect often associated with the Dead Sea Scrolls community at Qumran. He notes that the Essenes possessed **secret books** containing the names of angels and arcane knowledge, which initiates swore oaths to protect. These books were not to be revealed to outsiders. The Essene practice of encoding esoteric knowledge in texts accessible only to initiates is a form of **community-based secrecy** — the precursor to the cryptographic distinction between those who possess the key and those who do not.

Josephus also describes how the Essenes required new members to swear "that he will keep the books of the sect, and the names of the angels, secret." This is one of the earliest documented instances of a formal oath of cryptographic secrecy in Western literature.

### The Zealots' Coded Messages

In *Bellum Judaicum* Book 4, Josephus reports that the Zealot factions within besieged Jerusalem communicated through a system of **pre-arranged signals and passwords**. When the Idumeans (Edomites) were summoned to Jerusalem to assist one Zealot faction against another, the communication was conducted through secret messengers who used agreed-upon recognition signals. Josephus does not describe the code in detail, but the scenario — rival factions within a besieged city using secret communication to coordinate — is exactly the kind of practical cryptographic problem *Mercury* addresses.

### The Masada Defenders

Josephus's account of the siege of Masada (Book 7) describes the defenders' communication methods during the final Roman assault. Though Josephus does not detail cipher systems, the scenario of a besieged fortress needing to coordinate defence through signals is directly relevant to the signalling chapters of *Mercury* (torches, smoke, bells).

## Josephus as a Source for 17th-Century Scholars

Josephus was among the most widely read classical historians in 17th-century England. His works were available in multiple editions:

- The **Greek text**, edited and published throughout the 16th and 17th centuries
- **Latin translations**, the standard scholarly medium
- **English translations**: Thomas Lodge's translation (1602) was widely available; a new translation by Sir Roger L'Estrange would appear in the decades after *Mercury*

For Wilkins and his contemporaries, Josephus was not an obscure specialist source but a **standard classical authority**, as familiar as Herodotus or Tacitus. His eyewitness account of the Jewish War carried special weight because he had been a participant — a commander on the Jewish side before his capture and defection. When Wilkins cites Josephus for the swallowed-gold story and the Jotapata messengers, he is drawing on a source his readers would recognise.

## Connection to Porta's Navarre Story

Wilkins pairs the Josephus swallowed-gold story with [[porta-baptista|Porta's]] account of a man at the siege of Navarre who swallowed a box containing a letter. Both involve ingestion and subsequent recovery; both involve siege conditions; both represent the extreme end of physical steganography. Together, they form a matched pair of **ingestion narratives** — the ultimate bodily concealment. Wilkins's point is that both were desperate measures made necessary by ignorance of cryptographic technique. Learn ciphers, avoid indigestion.

## Historical Significance for Cryptography

Josephus's significance for the history of cryptography is indirect but real:

1. **Vivid illustration**: The swallowed-gold story gives *Mercury* one of its most memorable passages, conveying the stakes of failed secrecy with visceral power.

2. **Source for steganographic extremes**: Josephus provides first-century evidence that people will go to extraordinary physical lengths to conceal valuable objects — the same instinct that drives cryptographic innovation.

3. **Evidence of institutional secrecy**: Josephus's accounts of Essene secret books and Zealot coded messages document early organised practices of information control — the social infrastructure within which cryptographic techniques develop.

4. **Authority for historical depth**: By citing Josephus, Wilkins demonstrates that secret communication is not a modern (and therefore suspicious) invention but an ancient human practice with classical precedent.

## Cross-References

- [[mercury-wilkins]] — *Mercury*, Chapter 4
- [[ch-4-secret-conveyances]] — the chapter where the gold-swallowing and Jotapata stories appear
- [[porta-baptista]] — the parallel Navarre story
- [[john-wilkins]] — the author who mined classical sources for cryptographic anecdotes
- [[history-of-cryptography]] — wider historical context
