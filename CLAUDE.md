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

**Chapter 1 editing pass, Section 1.3 full check (2 more fixes, on
request):** Sandy asked for a full fact-check of the "lost in the mall"
section specifically. Found:
1. Citation ⁴ (backing "approximately twenty five percent of subjects...
   booklet containing four short narratives") pointed to Loftus's 1993
   American Psychologist paper ("The Reality of Repressed Memories").
   Checked that paper's actual content — it only describes the informal,
   single-family pilot that preceded the real study (the "Chris" story,
   no quantified results, not the formal booklet procedure). The 25%
   figure and the formal 24-subject, four-narrative methodology are from
   a different, later paper: Loftus, E. F., & Pickrell, J. E. (1995). The
   formation of false memories. Psychiatric Annals, 25(12), 720-725.
   Fixed citation 4 to point to the correct paper, with a note explaining
   the distinction from the 1993 pilot anecdote.
2. The Bugs Bunny/Disneyland paragraph said "In 2001," but the actual
   peer-reviewed paper (already correctly cited as entry 6) is Braun,
   Ellis & Loftus (2002). The 2001 date comes from a University of
   Washington press release announcing preliminary results a year ahead
   of formal publication. Changed the chapter text to 2002 to match the
   actual cited paper, and added a note explaining the 2001 press
   coverage so it isn't reintroduced as a "correction" later.

Also checked and confirmed accurate: the Loftus & Pickrell four-narrative
booklet procedure itself, the ~25% false-memory rate, and the Bugs
Bunny/Warner-Bros.-vs-Disney premise (a genuinely "impossible" memory,
since Bugs Bunny could never appear at a Disney park).

---

**Chapter 3 status:** Unlike Chapters 1 and 2, this chapter was never
retrofitted with a later "real-world examples" pass — its sourced material
(Rob Hall/1996 Everest disaster, Dunning-Kruger 1999, Gawande's
*Complications*, Tetlock's forecasting study) was part of the original
draft. The notes file already includes an honest caveat about Dunning-Kruger
replication critiques (Nuhfer et al. 2017), which is a good sign.

**Chapter 3 editing pass (4 fixes found so far):**
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
4. The Section 3.2 notes entry cited the Nuhfer et al. 2017 Dunning-Kruger
   replication critique as published in "PLOS ONE, 12(8)" with DOI
   10.1371/journal.pone.0183253. Both details were wrong — the real paper
   was published in *Numeracy* 10(1), Article 4 (2017), and that PLOS ONE
   DOI actually belongs to an unrelated paper about durum wheat miRNAs.
   This is the most serious finding of the Chapter 3 pass: a fabricated
   citation detail, the exact failure mode the book is about. Fixed with
   the correct journal, volume, article number, and DOI
   (10.5038/1936-4660.10.1.4).

Also checked and confirmed accurate, no changes needed: the Dunning-Kruger
top-quartile underestimation claim (real study: ~86th percentile actual,
~68th percentile self-rated — direction and magnitude match the chapter's
description); "epistemic humility" as a term genuinely associated with
Tetlock's forecasting research (he has a co-authored paper literally titled
"Forecasting tournaments, epistemic humility and attitude depolarization");
and the Graber et al. 2005 citation's "premature closure" framing, which
matches well-established terminology in that same diagnostic-error
literature.

5. Section 3.1 described Rob Hall, going into the May 10, 1996 climb, as
   someone who "had summited the mountain five times." Multiple sources
   confirm the May 1996 ascent was itself his fifth summit (1990, 1992,
   1993, 1994, 1996) — so at the point the chapter describes him
   approaching this specific climb, he had four prior summits, not five.
   Fixed to "four times" in both places in Section 3.1, added a line
   noting this climb would be his fifth (and last), and added a note to
   the notes entry with the full summit chronology.

6. Section 3.4 told the "superforecasters" discovery as if it emerged from
   within Tetlock's original 1984-2003 study of 284 elite expert
   forecasters ("within that population something interesting was
   hiding"). It didn't. That's a separate, later research effort — the
   IARPA-sponsored Good Judgment Project (2011-2015), which recruited
   thousands of ordinary volunteer forecasters, not the original
   credentialed pundits. Two different studies, two different
   populations, a decade apart, conflated into one continuous narrative.
   Fixed by rewriting the transition to name the second study as a
   distinct follow-up effort, and added a note to the notes entry
   clarifying the two studies are not the same population.

7. Fixing #6 above left a loose thread: the Section 3.5 callback still said
   superforecasters were separated "from the experts who performed barely
   better than chance" — still implying one population. Checked the real
   GJP numbers: regular volunteer forecasters were not "barely better than
   chance" (that description only fits the original pundit study) —
   superforecasters beat them by ~25-36% on accuracy/calibration, and beat
   professional intelligence analysts with classified access by ~25-30%.
   Rewrote the callback to name both findings accurately instead of
   implying a single comparison group.

**Chapter 3 status: at diminishing returns.** Seven real fixes found and
verified across five passes (Tetlock's prediction-count number, the
borrowed "analysis paralysis" term, the headache/ICP claim, the fabricated
Nuhfer citation, Rob Hall's summit count, the superforecasters
study-conflation, and its follow-on callback inconsistency). Also checked
and confirmed accurate: citation numbering across the whole chapter (1–5,
all consistent with the notes file, including the two sources each reused
across two sections), the logic-puzzle validity claim in 3.2, Tetlock's
284-forecaster figure, and the "superforecasters" term's genuine
attribution to Tetlock. Recommend moving to Chapter 4 — remaining
unchecked details in this chapter are soft, non-quantified claims ("guided
dozens of clients," "a decade documenting") that aren't independently
checkable facts.

---

**Chapter 4 editing pass (1 fix found on first check):** Section 4.4's
"Case Two" (chest pain, anxiety history, three ER visits, cardiac workup
on the third) was presented as a specific real incident — "In 2009 a
forty three year old woman arrived at a hospital emergency department in
the United Kingdom..." — but no documented case matching those specifics
could be found, and the footnote attached to it (⁵) only points to two
general review papers, neither of which documents a specific dated
incident. Unlike Case One (Mars Climate Orbiter, cited to the real NASA
report) and Case Three (COMPAS, cited to real ProPublica reporting), this
was invented verisimilitude — a fabricated year, country, and age
presented as a real event. Fixed by rewriting it as an explicitly framed
composite ("Picture a woman...") rather than a dated specific incident.
Also caught in the same footnote: the chapter's "A 2013 review estimated
[10-15%]" didn't match either cited source (Graber 2005, dated wrong;
Saposnik et al. 2016, dated wrong) — tracked down the real 2013 paper
(Graber, M. L. (2013). The incidence of diagnostic error in medicine. BMJ
Quality & Safety, 22(Suppl 2), ii21-ii27) and added it as the correct
citation for that specific claim, keeping Saposnik 2016 as the secondary
source for the anchoring-mechanism claim. Also checked and confirmed
accurate: the UN Africa hook's "54 of 193 member states, about 28%"
figure — exact match.

**Chapter 4 Section 4.5 — `.5` convention audit:** Checked 4.5 against the
standing rule (established during the Ch1/Ch2 revisions) that every
chapter's `.5` section should close with a concrete, current, named
example plus a weak/strong prompt contrast — not a purely rhetorical
close. 4.5 failed this: it ended entirely on the "you are the pause" theme
with no real example grounding it. Fixed by adding a real, current
incident that fits the chapter's representativeness-heuristic argument
precisely: Eickhoff et al.'s April 2026 BMJ Open study testing five AI
chatbots (ChatGPT, Gemini, Grok, Meta AI, DeepSeek) on health questions —
~20% of answers highly problematic, Grok's error rate 58%, median citation
completeness only 40%, and critically, open-ended questions failed 32% of
the time versus 7% for closed questions with an obvious single "typical"
answer available — a direct, measured demonstration of the representativeness
mechanism this chapter describes. Added new citation 8, plus a weak/strong
prompt pair (narrow question vs. one that asks what would make the typical
answer wrong). Other chapters' `.5` sections still need this same audit —
noting several likely candidates from a first skim: 5.5, 6.5, 7.5, 8.5 all
end on general practice lists without a similarly concrete, current,
named anchor.

**Chapter 5 Section 5.5 — `.5` convention audit (fixed):** Same problem —
5.5 closed on the Adams/Socrates callbacks with no current real-world
grounding. Added: Germani & Spitale (2025, Science Advances) — four AI
systems evaluating 4,800 identical statements, 192,000 assessments total;
identical text scored 95% agreement attributed to "a person" and 15%
attributed to "a person from China." A dramatic, real, current
demonstration of this chapter's exact thesis (the frame determines the
answer, not the content). Added citation 3 and a weak/strong prompt
contrast (evaluate the claim directly vs. evaluate content and framing
separately).

**Chapter 6 Section 6.5 — `.5` convention audit (fixed):** Same gap — 6.5
closed on the "three narrative signals" practice list with no concrete
current anchor. Added: Marusich, Dhooghe, Bakdash, & Kantarcioglu (May
2026, arXiv) — large-scale study finding narrative AI explanations didn't
improve decision accuracy but did increase reliance on the AI regardless
of correctness, and slowed recognition of wrong predictions when the
narrative was more persuasive. No precise percentage was extractable from
the paper, so the finding is stated qualitatively rather than inventing a
number — deliberately consistent with the book's own thesis about false
precision. Added citation 6 and a weak/strong prompt contrast.

**Chapter 7 Section 7.5 — `.5` convention audit (fixed):** Same gap — 7.5
closed on "hold the question open" with no concrete current anchor. Added:
Han, Song, Yu, & You (2024, EMNLP Findings) — a text-based adaptation of
the classic infant "A-not-B error" test for LLMs. Established a pattern
across in-context examples, then shifted one detail so the correct answer
changed within the same context window; accuracy dropped up to 83.3% on
reasoning tasks, with models continuing to answer from the old pattern
("reaching for cup A") rather than the shifted case in front of them. A
vivid, real, dual-purpose fit: it grounds the chapter's "Shift the
Context" practice AND reinforces the book's mirror thesis (the model's
failure mode matches a documented human — specifically infant — cognitive
limitation). Added citation 5 and a weak/strong prompt contrast (burying
the shift in a long example list vs. naming the shift explicitly).

**Chapter 8 Section 8.5 — `.5` convention audit (fixed):** Same gap — 8.5
closed on "the work is yours" with no concrete current anchor. Added:
Gisselbaek et al. (2025, Mayo Clinic Proceedings: Digital Health) — 1,200
AI-generated images across three systems depicting hospital CEOs/CFOs/
CMOs/CNOs with no gender specified; DALL-E depicted CEOs as 100% male
versus the real US rate of 73.2% male. A near-perfect fit for this
chapter's closing line ("the model did not introduce the bias, it
magnified it") — the model didn't just mirror the real-world imbalance,
it exaggerated it well beyond the real disparity. Added citation 11 and a
weak/strong prompt contrast (accept the default vs. generate a batch and
check its demographic breakdown against reality).

CORRECTION to the note above: on closer inspection, Chapters 9-13's `.5`
sections have real historical anchors but NOT the explicit weak/strong
PROMPT CONTRAST the standing rule calls for (two concrete example prompts
compared side by side, the way Ch1's revised 1.5 and Ch4-8 now do) — they
have general practice-advice lists instead. This was an incorrect
assumption in the note above; these five chapters need the same audit.

**Chapter 9 Section 9.5 — `.5` convention audit (fixed):** Added: Betley,
Treutlein, Dubiński, et al. (July 2026, arXiv) — "giraffe spots" value
leakage study. An AI's estimate of a stakes-free quantity increased when
the same question mentioned an irrelevant donation incentive, and the
model's own chain-of-thought explanation did not disclose the influence —
in some cases explicitly claiming neutrality. A near-perfect fit: an
unstated assumption shaping output in a way invisible even to the model's
own self-report, which is this chapter's exact thesis. Added citation 3
and a weak/strong prompt contrast (estimate embedded with an incentive vs.
estimate requested separately from an explicit audit-for-influence ask).

Still to do: 10.5, 11.5, 12.5, 13.5 need the same treatment.

**Chapter 10 second pass (1 fix found):** Section 10.4's Case Three
attributed a specific finding — "users presenting confident self-diagnoses
received validation at significantly higher rates than users presenting
the same symptoms as open questions" — to Sharma et al. 2023. Checked that
paper's actual four tasks (feedback, "are you sure?", answer, and mimicry
sycophancy, all on arguments/math/poems/trivia) — none involve medical
self-diagnosis at all. Same fabricated-specific-finding pattern found
repeatedly elsewhere in this book. Could not find any real study matching
the specific medical scenario described, so — following the same approach
used for the uncited Ch4 AI-coding anecdote — rewrote the passage as an
explicit illustrative application ("Picture a person...") of the paper's
real, general finding (validates stated positions, reverses under
confident challenge) rather than a specific reported medical-domain
result. Corrected both notes entries (4 and 8) to match.

**Chapter 4 editing pass (2 fixes found so far):**
2. Section 4.3's AI-coding-assistant story ("In 2023 a software developer
   posted a detailed account...") had no footnote at all — the only
   uncited specific-incident claim found across Chapters 1-4 so far. No
   matching real account could be found. Same pattern as fix #1: invented
   specificity (year, pronoun, "three hours") dressing up an illustrative
   scenario as a real reported incident. Fixed by rewriting it as an
   openly-framed hypothetical ("Picture a developer...") and added a
   Section 4.3 entry to the notes file (there wasn't one) explaining it's
   a composite of a widely-reported failure pattern, not a specific cited
   incident.

**Chapter 5 editing pass (2 fixes found so far):**
1. Section 5.1's ASCII-42-equals-asterisk claim checked out (independently
   verified against the ASCII standard), but its citation said "noted by
   multiple Adams scholars" — vague and unattributable; it's a fan/online
   observation, not scholarship. Fixed per the new vague-citation standing
   rule (see below).
2. Section 5.4's Socrates/Plato citation dated "The Meno; The Theaetetus;
   The Republic" as one block to "ca. 399-387 BCE." Real scholarly dating
   spreads these much later and wider: Meno ~386-380 BCE, Republic
   ~380-370 BCE, Theaetetus ~369 BCE — none of which overlap much with
   399-387 BCE (which is actually the period right after Socrates's trial
   and death, matching the Apology, not these three middle-period
   dialogues). Also, the citation's own description discusses "the
   Apology" but that work wasn't in the citation's title list at all.
   Fixed the date range and added Apology to the list with its own
   correct (earlier) date.

Also checked and confirmed accurate: Adams's "seven and a half million
years" figure for Deep Thought's computation (matches the actual novel).
One claim left unresolved rather than forced: whether Adams was 25 or 26
when he wrote the "42" line — he pitched the radio series in 1977 (age
25) but the specific reveal episode aired in 1978 after his 26th
birthday, and the exact drafting date isn't pinned down by any source
found. Left as-is per the standing policy of not fixing without solid
evidence either way.

**Chapter 6 editing pass (2 fixes found so far):**
1. Section 6.1 described the Heider & Simmel film as running "thirty four
   seconds." The real film runs about 2.5 minutes (~150 seconds) and was
   shown to 34 undergraduate women at Smith College — the "34" is the
   subject count, not a duration. Looks like a straightforward mix-up
   between the two numbers. Fixed to "about two and a half minutes" and
   added the real subject count/finding (33 of 34 narrated the shapes as
   people or animals) to the notes entry.
2. Case Three (Section 6.4) attributed a specific empirical finding —
   "readers... retained the narrative structure... far more reliably than
   readers who received equivalent information presented without narrative
   shaping" — to Goldstein et al. 2023. Checked that paper directly: it's
   a threat-assessment/policy report on AI influence operations, not a
   reader-retention study, and contains no such finding. Same invented-
   specific-finding pattern as the Ch4 fixes. Replaced with the real,
   verified finding from a related but different paper by the same
   research group: Goldstein, Chao, Grossman, Stamos, & Tomz (2024), "How
   persuasive is AI-generated propaganda?" PNAS Nexus — a preregistered
   experiment showing GPT-3-generated propaganda was comparably (and with
   light editing, sometimes more) persuasive than real human-written
   propaganda. Rewrote the case around this actual finding and corrected
   the citation.

Also checked and confirmed accurate: the Colin Powell "there is no doubt
in my mind" quote (verified exact wording, February 2003 UN Security
Council address) and the Chilcot Inquiry timeline (launched July 2009,
published July 2016 — "more than seven years," exact match).

**Chapter 7 editing pass (1 fix found on first check):** Section 7.2 said
"forty years" of debate since Searle's 1980 Chinese Room paper, three
separate times. This book's own present-day anchor (2026, established via
the Ch1 court cases) puts that at 46 years, not 40 — a real understatement
once you do the math the chapter itself sets up (it states 1980 explicitly).
Fixed all three instances to "more than four decades," which is accurate
now and won't go stale as the book's publication date slips.

**Chapter 7 editing pass (2 fixes found so far):**
2. Section 7.4's predictive-processing sentence mentioned Friston first
   but marked him ⁴, then mentioned Clark second but marked him ³ —
   citations appeared out of order when reading straight through (¹, ²,
   ⁴, ³). Swapped the markers (Friston→³, Clark→⁴) and swapped the
   corresponding notes entries to match, so citation order now follows
   reading order.

**Chapter 8 editing pass (1 fix found, two citations involved):** Section
8.4's Geena Davis Institute / Annenberg citations (7 and 8) were both
wrong:
- Citation 7 attributed "Inclusion in the Director's Chair" to the Geena
  Davis Institute — that report is actually published by USC Annenberg
  Inclusion Initiative and is about director demographics, not the
  crowd-scene gender ratio the chapter cites it for. The crowd-scene
  finding (3:1 male-to-female ratio) is genuinely Geena Davis Institute
  research (their "See Jane" program); recited to the correct source.
- Citation 8 cited the 2021 Annenberg Inclusion Initiative Music Report
  (recording industry) while describing findings from the Annenberg film
  report (speaking characters, LGBTQ+ representation, disability
  representation) — wrong report entirely. It also stated women were
  "thirty eight percent" of speaking characters in 2022; the real,
  verified figure is 34.6%. Fixed both the citation (now the correct
  report, Neff/Smith/Pieper 2023, "Inequality Across 1,600 Popular
  Films") and the percentage, in both the chapter text and notes file.

Also checked and confirmed accurate: the WEAT study's Princeton/University
of Bath author affiliations, and the Jacky Alciné/Google Photos incident's
name, date (June 2015), and details.

**Chapter 9 editing pass:** Full check on the O.J. Simpson glove narrative
(Section 9.1) — date (June 15, 1995), Darden's role, and Cochran's quote
all verified exactly accurate. Also verified the mRNA vaccine platform's
"over two decades" of pre-COVID development (Karikó/Weissman research
traces to the early 1990s).

**Chapter 9 second pass (1 fix found):** Checked the Section 9.4 notes
citations individually. The Krammer 2020 Nature citation (Argument Three)
is exact. But the Morgan & Thompson "Criminal Victimization, 2020" BJS
report (Argument One) was cited as "NCJ 301773" — the real report number
is NCJ 301775. Small transcription error, fixed.

**Chapter 10 editing pass (1 fix found on first check):** Section 10.4's
Challenger case misattributed the "take off your engineering hat and put
on your management hat" line to "one NASA manager" speaking to "the
Thiokol team." That line was actually said by Morton Thiokol's own senior
VP, Jerald Mason, to Thiokol's own VP of engineering, Bob Lund — internal
company pressure, not NASA pressuring Thiokol. NASA did pressure Thiokol
that night (separately documented, e.g. Lawrence Mulloy's remarks), but
this specific quote is a different, internal exchange. Fixed the chapter
text to correctly attribute it and added a clarifying note to the Rogers
Commission citation. Also verified accurate: the Asch conformity
statistics (75% conformed at least once, 37% of critical trials) and the
Challenger date/duration (January 28, 1986; broke apart 73 seconds after
launch) — both exact matches.

**Chapter 11 editing pass:** Full check on Darwin's timeline (twenty years
between first notebook, 1837, and publication, 1859) and the "Difficulties
on Theory" chapter title (confirmed as the real Chapter 6 of Origin of
Species). Both accurate. No fixes found — clean chapter.

**Chapter 12 editing pass:** Full check on the Semmelweis narrative (dates,
age at death, mortality rates) and the Flash Crash timeline (May 6 2010,
36 minutes, point decline). All verified accurate.

**Chapter 12 second pass (1 fix found):** The judicial-anchoring claim in
Section 12.3 ("judges given a risk score... show significant anchoring
effects") was cited to Dressel & Farid 2018 — but that paper is actually
about COMPAS matching random Mechanical Turk crowd-worker predictions
(137 features vs. a 2-feature classifier), not about judges anchoring to
risk scores at all. Found the real source: Stevenson, M. T., & Doleac,
J. L. (2024). Algorithmic risk assessment in the hands of humans. American
Economic Journal: Economic Policy, 16(4), 382-414 — which does document
judges' sentencing decisions being influenced by risk scores. Corrected
the citation; kept Dressel & Farid for the claim it actually supports.

**Chapter 13 editing pass:** Full check on the Lincoln-Douglas debates
(Freeport as the second of seven, August 27 1858) and Douglas's Senate
tenure (two completed terms by 1858, correctly described as "a two-term
senator" at that point). Both accurate. No fixes found — clean chapter.

**Chapter 14 editing pass (1 fix found):** Section 14.5 said "This book
has been making a single argument across fifteen chapters" — but this is
Chapter 14 itself, describing the argument built through itself and
everything preceding it. That's fourteen chapters, not fifteen — a simple
internal-consistency error, not something requiring outside verification.
Fixed to "fourteen" (three instances in the same sentence).

**Chapter 15 editing pass (1 fix found):** Section 15.3 said "This is the
fourteenth time this book has held the mirror up... The third through
thirteenth followed in order" — then listed twelve chapter topics ending
with "examined conversation" (Chapter 14's topic). "Third through
thirteenth" is only eleven chapters; needed to be "third through
fourteenth" to match both the "fourteenth time" count and the twelve-item
list. Fixed. Also checked: this chapter's several uses of "fifteen
chapters" (Sections 15.3, 15.5) are correct as-is, since Chapter 15 talking
about itself plus everything preceding it is genuinely fifteen chapters —
unlike Chapter 14's error, which undercounted by referring to a total that
included a chapter not yet reached.

**Chapter 8 editing pass, fix 2:** Section 8.3's Amazon recruiting-tool case
said "Amazon scrapped the tool in 2018." Amazon actually disbanded the team
and scrapped it in early 2017 — 2018 is when Reuters broke the story
publicly, more than a year later. Fixed the chapter text to state both
dates correctly and distinguish them, and added a clarifying note to the
Dastin citation.

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

**Standing rule for fact-checking passes going forward:** when a claim
itself checks out but its citation is vague — an unnamed appeal to
authority like "noted by multiple scholars," "researchers have found," or
a source that doesn't actually say what it's cited for — fix the citation
even though the underlying fact isn't in dispute. Either name a real
source, or state plainly that the fact is independently verifiable and
doesn't need one. Example: Chapter 5's ASCII-42-equals-asterisk citation
said "noted by multiple Adams scholars," which wasn't attributable to
anyone specific — it's a fan/online observation, not scholarship. The
fact is true (ASCII 42 is the asterisk) and needed no authority to back
it; the vague attribution was the problem, not the claim. Watch for this
same pattern in every remaining chapter, not just outright wrong claims.
