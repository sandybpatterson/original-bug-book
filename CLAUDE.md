# THE ORIGINAL BUG – PROJECT HANDOFF
### For Claude: Read this first before doing anything else.

---

## What This Project Is

*The Original Bug: Human Cognition and the AI It Corrupted* is a completed first-draft nonfiction book by Sandy B. Patterson (he/they). The author's name is always written in full — never abbreviated.

The book argues that every flaw identified in AI — hallucination, overconfidence, pattern obsession, bias, narrative dependency, sycophancy — has a precise counterpart in human cognition, because AI was trained on human output. The machine is a mirror. The reflection is accurate.

The book has 16 chapters plus a prologue. Chapter 16 closes the book by scaling the argument from the individual to the civilizational.

---

## Current File Situation

The book exists in multiple formats in various states of completion. The goal of the current work session is to produce one clean markdown (.md) file per chapter, ready for GitHub.

### Already done as clean markdown:
- `TOB_Chapter1_Complete.md` ✓
- `TOB_Chapter2_Complete.md` ✓
- `TOB_Chapter16_Complete.md` ✓

### Exist as docx only — need to be converted to clean markdown:
- `TOB_Chapter3_Complete.docx`
- `TOB_Chapter4_Complete.docx`
- `TOB_Chapter5_Complete.docx`
- `TOB_Chapter6_Complete.docx`
- `TOB_Chapter7_Complete.docx`
- `TOB_Chapter8_Complete.docx`
- `TOB_Chapter9_Complete.docx`
- `TOB_Chapter10_Complete.docx`
- `TOB_Chapter11_Complete.docx`
- `TOB_Chapter12_Complete.docx`
- `TOB_Chapter13_Complete.docx`
- `TOB_Chapter14_Complete.docx`
- `TOB_Chapter15_Complete.docx`

### Source files (HTML sections) also exist for most chapters if needed.

---

## The Markdown Format Standard

Use `TOB_Chapter1_Complete.md` and `TOB_Chapter2_Complete.md` as the canonical style reference. Every chapter must match this format exactly.

### Key formatting rules:

**Header:**
```
# THE ORIGINAL BUG
### Chapter N — Chapter Title
```

**Section breaks between sections:**
```
---
## Section N.X — Section Title
```

**Section dividers within sections** (three spaced asterisks, escaped):
```
\* \* \*
```

**Pull quotes** (blockquote format):
```
> Text of the pull quote here.
```

**Exercise/exhibit boxes** (bold label, then content):
```
**Label Text**

Content here, indented or as regular paragraphs.
```

**AI transcript boxes:**
```
**AI Assistant — Response Transcript**

*User: the question here*

The AI response here as a regular paragraph.
```

**Superscript citations** — Unicode superscript characters inline at the point of the sourced claim:
¹ ² ³ ⁴ ⁵ ⁶ ⁷ ⁸ ⁹

Example: `...the study was conducted in 1999.²`

**No inline sources sections** — sources do NOT appear at the bottom of each chapter section. All sources live in the separate notes document.

**Footer at end of each chapter:**
```
---

*The Original Bug — Chapter N: Chapter Title — Sandy B. Patterson*
```

---

## The Citations / Notes Document

`TOB_Notes_and_Sources.txt` is the end-of-book sources document. It already contains entries for Chapters 1, 2, 3, and 4.

When converting a chapter to markdown:
1. Add superscript numbers at every specific empirical claim in the prose
2. Add corresponding entries to `TOB_Notes_and_Sources.txt` in chapter order
3. Do NOT add a sources section to the chapter file itself

Format for notes entries:
```
================================================================================
CHAPTER N — CHAPTER TITLE
================================================================================

Section N.X — Section Title

1. Brief description of claim: Author, A. (Year). Title. Publisher.
URL if available.

One or two sentences of context about what this source establishes
and why it matters to the claim being cited.
```

---

## Chapters with Known Sources to Cite

Here are the key sourced claims per chapter that need superscript markers:

**Chapter 5** — Ask a Better Question
- Douglas Adams / Deep Thought / Hitchhiker's Guide (1979)
- Plato's Socratic dialogues (Meno, Theaetetus, Republic)

**Chapter 6** — Narrative Is Not Truth
- Heider & Simmel 1944 animated shapes study
- Buckner et al. 2008 default mode network
- Iraq Inquiry (Chilcot Report) 2016
- Loftus 1993 recovered memory
- Goldstein et al. 2023 AI misinformation

**Chapter 7** — What Does Understanding Even Mean
- Perfetti & Stafura 2014 reading comprehension
- Searle 1980 Chinese Room
- Clark 2016 predictive processing
- Friston 2010 free energy principle

**Chapter 8** — The Bias Mirror (this chapter already has inline sources in the docx — strip them out of the chapter text and move them to the notes document with superscripts in the prose)
- Caliskan et al. 2017 WEAT study
- Cirillo et al. 2020 medical AI sex/gender bias
- Bender et al. 2021 Stochastic Parrots
- Amazon recruiting tool (Dastin 2018 Reuters)
- Google Photos gorilla (Simonite 2018 Wired)
- ProPublica COMPAS (Angwin et al. 2016)
- Geena Davis Institute 2020
- Annenberg Inclusion Initiative 2022
- Noble 2018 Algorithms of Oppression
- Buolamwini & Gebru 2018 Gender Shades

**Chapter 9** — The Examined Assumption
- Morgan & Thompson 2021 BJS crime data
- Krammer 2020 Nature mRNA vaccines
- Angwin et al. 2016 ProPublica COMPAS (again)

**Chapter 10** — The Social Animal and Its Machine
- Asch 1951 conformity experiments
- Tourangeau & Yan 2007 social desirability bias
- Ashford & Blatt 2003 sycophancy in organizations
- Sharma et al. 2023 AI sycophancy
- Ouyang et al. 2022 RLHF training
- Challenger Rogers Commission 1986
- Ptacek & Eberhardt 1996 breaking bad news
- Sharma et al. 2023 (again, medical sycophancy)

**Chapter 11** — The Art of Being Wrong Productively
- Darwin autobiography 1887
- Kunda 1990 motivated reasoning
- Lord, Ross & Lepper 1979 biased assimilation
- Arkes et al. 1988 hindsight bias
- Gollwitzer 1999 implementation intentions
- Guo et al. 2022 automated fact-checking limits

**Chapter 12** — When Certainty Kills
- Semmelweis / Nuland 2003
- Reason 1990 Human Error
- Taleb 2007 Black Swan
- Topol 2019 deep learning medicine
- Goddard et al. 2012 automation bias
- SEC/CFTC Flash Crash report 2010
- Dressel & Farid 2018 COMPAS accuracy
- Obermeyer et al. 2019 racial bias health algorithm
- Shumailov et al. 2023 model collapse
- Lo 2004 adaptive markets

**Chapters 13, 14, 15** — lighter sourcing, confirm as needed:
- Ch 13: Holzer 1993 Lincoln-Douglas; Mill 1859 On Liberty; Walton 1996; Bail et al. 2018; Perez-Ortiz et al. 2023
- Ch 14, 15: likely minimal new citations needed — these are synthesis chapters

**Chapter 16** — We Are the Training Data (already clean markdown, needs sources added)
- Common Crawl documentation
- Shumailov et al. 2023 model collapse (already in Ch 12)
- Open Science Collaboration 2015 replication crisis
- Copernicus / Galileo (historical, light citation)
- Suffrage movement (historical, light citation)

---

## What Good Output Looks Like

For each chapter, produce:
1. A clean `.md` file named `TOB_Chapter[N]_Complete.md`
2. Matching entries added to `TOB_Notes_and_Sources.txt`

Check your work against `TOB_Chapter1_Complete.md` — if it looks like that, it is correct.

---

## The Author

Sandy B. Patterson (he/they). Full name always. Never "Sandy Patterson," never "S.B. Patterson," never abbreviated in any form.

---

## What Is NOT Needed Right Now

- Front matter (acknowledgments, author note, index) — later
- GitHub upload — later
- Volume Two drafting — later
- Docx files — the markdown files replace them

---

## Priority Order

Convert chapters in this order, one at a time, confirming each before proceeding:

3 → 4 → 5 → 6 → 7 → 8 → 9 → 10 → 11 → 12 → 13 → 14 → 15 → Prologue → 16 (add sources only)

Start with Chapter 3. When done, say so and wait for confirmation before continuing to Chapter 4.
