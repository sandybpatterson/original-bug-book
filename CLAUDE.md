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

## Status

All 16 chapters plus the prologue are complete as clean markdown and wired
into `chapter.html`. The docx-to-markdown conversion work this file originally
tracked is done — there is no unconverted chapter left.

**Known-good:** Chapter 2 checked against every item in this file's format
standard (header, section breaks, dividers, pull quotes, exhibit boxes, AI
transcript box, superscript citations, no inline sources, footer) — passes
cleanly, citations 1–9 all have matching entries in `TOB_Notes_and_Sources.txt`.

**Chapter 2 editing pass complete (3 fixes, in order found):**
1. Section 2.4's AI transcript example claimed a second cortisol peak in
   early afternoon — not well-established circadian science. Tightened to
   the real, single morning peak.
2. Section 2.2's hot-hand fallacy passage cited Gilovich et al. (1985) as
   settled proof of an illusory pattern, without knowing Miller & Sanjurjo
   (Econometrica, 2018) later found a selection bias in that study's
   counting method and reversed the finding on reanalysis of the same data.
   Rewrote the passage to tell that story — strengthens the chapter's own
   thesis (scientists fell for a pattern-without-mechanism error too) rather
   than just fixing a stale citation.
3. The rewritten Section 2.5 ChatGPT-retraction passage initially credited
   Ben Williamson (University of Edinburgh) with catching the meta-analysis's
   pooling error. His verified public remarks were actually about the
   paper's post-publication virality, not the methodological critique —
   fixed by citing the retraction notice's own stated reason directly
   instead of an unverified named attribution.
4. The rewritten Section 2.2 hot-hand passage explained Miller & Sanjurjo's
   bias as an end-of-sequence truncation effect (streaks near the end have
   no "next" flip to check). That's not the actual mechanism — it's a
   search-procedure asymmetry (a run of hits gets consumed as one continuous
   chain, giving it fewer independent chances to be checked than isolated
   hits get). Corrected the explanation to match the real finding.

5. The new hot-hand passage in Section 2.2 closed with "real in its
   conviction and absent... from its foundation" — nearly verbatim duplicate
   of Section 2.5's pre-existing signature line ("real in its conviction,
   absent in its foundation"), diluting that line's impact by using it twice
   in one chapter. Gave 2.2 its own closing instead.
6. The Section 2.2 coin-flip example itself (`H H H H H T H H H H`) is 9
   heads and 1 tail — but the prose described it as "eight heads and two
   tails." This one predates all the fixes above; it was in the chapter's
   original text, not introduced by this editing pass. Fixed to "nine heads
   and one tail," matching the actual sequence shown.
7. The hot-hand passage restated "thirty-three years / three decades" four
   times across three short paragraphs, and one closing sentence
   substantively repeated a point the paragraph before it had already made
   (field-wide persistence of the wrong finding). Trimmed to state it once.

Note the pattern across fixes 2-5: each was introduced by the same editing
pass that added the real-world 2026 examples this file's ".5 section"
convention calls for. Real examples raise the stakes on getting every detail
right — verify mechanism, attribution, and citation separately, and check
new prose against the rest of the chapter for unintentional repetition —
before treating a passage as settled, per this chapter's own thesis. Fix 6
breaks that pattern — a reminder that original content deserves the same
scrutiny as new additions, not just spot-checks on what got added recently.

**Fixed:** Chapter 1's July 2026 revision (commit `8043001`, tightened prose
+ rewrote Section 1.5 with the 2026 court-sanction examples) cut a paragraph
that carried citation ³ but never renumbered the citations after it or removed
the now-orphaned source #3 (Barclay & Wellman) from the notes file. Citations
and notes entries have been renumbered contiguously (1–7) to fix this.

**Chapter 1 editing pass (1 fix found on request):** Section 1.5's "roughly
1,490 court proceedings worldwide" claim, cited from a public database, was
already stale the moment the July 17 revision used it — the database
(damiencharlotin.com/hallucinations, maintained by Damien Charlotin,
started April 2025, updates daily) had already reached 1,668 cases by
July 2, two weeks earlier. Fixed by reframing the claim around the fact
that the count climbs continuously rather than citing a number that goes
stale within weeks. Added citation 8 with a proper notes entry, including
an explicit note that any specific count cited should be treated as a
snapshot. Same risk applies to Chapter 2's ChatGPT-retraction stats
(486,000 views / 266 citations) — those are fixed historical facts about a
specific retracted paper, not a live counter, so they don't have this
problem, but worth remembering the distinction when adding future
real-world examples: is the cited number a frozen fact, or a live count
that will be wrong again in a month?

---

**Chapter 3 status:** Unlike Chapters 1 and 2, this chapter was never
retrofitted with a later "real-world examples" pass — its sourced material
(Rob Hall/1996 Everest disaster, Dunning-Kruger 1999, Gawande's
*Complications*, Tetlock's forecasting study) was part of the original
draft. The notes file already includes an honest caveat about Dunning-Kruger
replication critiques (Nuhfer et al. 2017), which is a good sign.

**Chapter 3 editing pass (2 fixes found so far):**
1. Section 3.4 stated Tetlock's 20-year study produced "nearly twenty
   thousand predictions" — the well-documented, widely-cited figure is
   82,361 forecasts by 2003, understating the real number by more than 4x.
   Fixed in both the chapter text and the notes entry. Verified separately:
   the Rob Hall/Everest timeline (4pm summit, two hours past the 2pm
   turnaround rule, Hansen's death on descent, the radio call to Hall's
   pregnant wife) is accurate as written — checked against multiple
   sources, no change needed.
2. Section 3.4 also described a surgeon's hesitation from over-knowledge as
   "a documented phenomenon in surgical decision-making sometimes called
   analysis paralysis," tied to the Gawande citation. That named term
   actually comes from a different body of research (Redelmeier & Shafir on
   choice overload — too many treatment options stalling a decision), not
   from an expert's own accumulated knowledge causing in-the-moment
   hesitation, which is what the chapter is actually describing. Gawande's
   book doesn't use the term either — the real parallel there is his essay
   "The Case of the Red Leg." Same pattern as the Ch2 Williamson
   misattribution: borrowing the authority of a real named phenomenon for a
   claim it doesn't actually document. Fixed by dropping the borrowed term
   from the chapter text and adding a note in the sources file explaining
   the distinction, so it isn't reintroduced later.
3. Section 3.3's AI-transcript rebuttal claimed a three-day unilateral
   headache with light sensitivity (no nausea) "can be a sign of increased
   intracranial pressure" and needs "same-day evaluation." Checked against
   actual clinical red-flag criteria (the SNOOP mnemonic: sudden/thunderclap
   onset, systemic symptoms like fever, neurologic signs, pattern change,
   age) and this presentation hits none of them — and elevated ICP
   headaches are classically bilateral with vomiting, not unilateral with
   photophobia, which is textbook migraine (unilateral in 60-70% of cases,
   lasting up to 3 days). The book's own rebuttal was the overconfident,
   unverified claim — the same failure mode the chapter warns about. Fixed
   by reframing the critique around what's actually true: the AI never
   asked the red-flag screening questions (sudden onset? fever? neuro
   signs? worst headache of your life?) that a clinician uses to rule out
   danger before settling on the likely answer — updated in the chapter
   text (Section 3.3 and the Section 3.5 callback) and added a note to the
   sources entry explaining the vignette is constructed so migraine is in
   fact the statistically correct answer; the failure is skipping the
   screening, not reaching the wrong conclusion.

**Resolved — and now a standing convention:** Chapter 1 Section 1.5's revision
replaced a repetitive/rhetorical ending with concrete, sourced, current
material — real 2026 court cases (Sixth Circuit, Nebraska Supreme Court) —
plus specific prompt-design advice, instead of just restating the thesis.
Chapter 2 Section 2.5 ("The Mechanism Question") has now been revised the
same way: its old rhetorical close ("Ask for it every time") was replaced
with a real, sourced 2026 case (the retracted ChatGPT-in-education
meta-analysis, g = 0.867 across 51 incompatible pooled studies, retracted
April 2026 — full citation is entry 8 under Section 2.5 in
`TOB_Notes_and_Sources.txt`) and a concrete before/after prompt contrast.

**Standing rule for every chapter's `.5` section going forward:** it should
end by teaching the reader a specific, concrete prompt-design principle
derived from that chapter's particular cognitive bug — framed as a contrast
between a weak prompt and a better one — grounded in a real, current, named
example (a real case, study, or incident with real numbers), not a rhetorical
restatement of the chapter's thesis. This is the throughline every `.5`
section should have: Chapter 1 → verification prompts for confabulation,
Chapter 2 → mechanism-probing prompts for pattern-without-cause. Apply the
same standard when writing or revising Chapters 3–16's `.5` sections.
