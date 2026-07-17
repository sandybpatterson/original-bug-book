# THE ORIGINAL BUG
### Chapter 1 — We Built It In Our Image

---

## Section 1.1 — The Brief

Steven Schwartz was not a reckless man. He had practiced law for more than three decades. He knew how to write a brief. He knew what courts expected and what judges tolerated and how much precision was required when you put a citation in front of a federal court in the Southern District of New York. He was not someone who cut corners. He was someone who had, over thirty years of practice, developed the kind of professional confidence that comes from having done a thing correctly so many times that doing it correctly feels automatic.

In the spring of 2023 he used an AI assistant to help research a personal injury case — Mata v. Avianca — and submitted a brief that cited more than half a dozen cases in support of his arguments. The cases had real-sounding names. Real-sounding docket numbers. Real legal reasoning threaded through the citations, connecting them to the argument at hand in ways that read like careful scholarship.

Not one of them existed.

The AI had invented them. All of them. Completely and with total confidence, in the fluent, authoritative language of someone who had located the cases, read them, and understood their relevance. When Judge P. Kevin Castel ordered Schwartz to produce copies of the cited cases, none could be found — because none were real. There were no transcripts to retrieve. No dockets to pull. No decisions to read. The cases were fictions dressed in the precise, technical vocabulary of legal fact, produced by a system that had never once flagged its own uncertainty.¹

Schwartz faced sanctions. The story made international headlines. The commentary that followed was swift and nearly unanimous: this was a cautionary tale about trusting artificial intelligence. Don't use AI for legal research without checking its work. The machine can be wrong. The machine can invent things. The machine cannot be trusted blindly.

All of that is correct. None of it is the point of this book.

\* \* \*

Here is what the headlines missed.

What Schwartz's AI did has a name. Not a technical name invented for the age of machine learning — a clinical name, decades old, borrowed from cognitive neuroscience, used originally to describe a specific symptom observed in patients with certain kinds of brain damage. The name is confabulation. And the reason it matters — the reason this book begins here, with this case, in this particular federal courthouse — is that confabulation is not something AI systems developed on their own. It is something they learned from us.

Confabulation was first documented in patients with damage to the frontal lobe or to memory systems. When asked about events they could not remember, these patients did not say they did not know. They produced detailed, confident, entirely invented accounts — and they believed every word of them. They were not lying. Lying requires knowing the truth and choosing to say something else. The confabulating patient had no access to the truth. The brain, confronted with a gap, did what it has always done. It filled the gap. It built a story. It served the story up as memory — with the full emotional and sensory texture of something genuinely recalled — because the brain does not experience the difference between a retrieved memory and a constructed one. It only experiences the output.

The AI in Schwartz's office did the same thing. Asked to find legal cases relevant to a particular argument, it encountered gaps in its training — cases it had not seen, precedents it could not locate. So it did what it had learned to do from the only source it had ever learned from. It filled the gaps. It constructed plausible-sounding outputs. It delivered them with the confidence of genuine recall. It confabulated.

> The AI did not malfunction. It did exactly what it had been trained to do — by the only teacher it ever had. And the teacher confabulates too. Every single day. Without knowing it is happening at all.

\* \* \*

The commentators who called the Schwartz case a cautionary tale about AI were right. But their caution stopped one step short of where it needed to go.

They treated confabulation as a flaw the machine had developed — something introduced in the engineering, something that distinguished the AI's unreliability from human reliability. What they did not examine was the prior question. Why does the machine do this? Where did it learn to? What, exactly, was it trained on — and what does the content of that training tell us about the nature of the flaw?

The training data that produced these models was generated almost entirely by human minds. Books written by humans. Articles written by humans. Legal briefs written by humans. Scientific papers, Wikipedia edits, forum posts, social media arguments — all of it produced by a species whose memory is reconstructive, whose confidence is routinely decoupled from its accuracy, and whose brains are in the business of gap-filling first and factual precision second.

We did not build a machine that confabulates and then compare it to a human mind that does not.

We built a machine that learned confabulation from beings who confabulate — and it learned the lesson completely.

That is what this book is about. And it starts — as all honest examinations do — with looking in the mirror.

---

## Section 1.2 — You Do This Too

Before this chapter goes any further, there is something you need to do. Not for the sake of illustration. Because what comes next will land differently if you have tried it first.

**An Exercise Before Reading Further**

If you have a sibling, think of one shared childhood memory — a birthday, a family trip, a fight, a moment you both found funny. Something you were both present for and have discussed at least once since.

Now ask yourself: do you remember it the same way? Not roughly the same way. The same way — the same details, the same sequence, the same account of who said what.

If you have ever compared notes with a sibling about a shared memory in any detail, you already know the answer. You do not remember it the same way. You may not even remember the same event. One of you remembers a vacation where something wonderful happened. The other remembers the same vacation and the wonderful thing simply is not there. You were in the same place at the same time. You have completely different memories of it.

This is not because one of you is lying or has a worse memory than the other. Memory is not a recording that two people make simultaneously and store in separate identical files. It is a reconstruction — assembled from fragments, shaped by emotion and attention, filled in at the gaps by whatever the brain finds most plausible.² Both reconstructions feel completely real. Both are, in important ways, partly invented.

> Memory is not a recording. It is a reconstruction — assembled from fragments, shaped by emotion and attention, filled in at the gaps by whatever the brain finds most plausible. Both siblings' versions feel completely real. Both are, in important ways, partly invented.

\* \* \*

Elizabeth Loftus spent her career making this visible in ways that could not be dismissed. Starting in the 1970s she began demonstrating, through controlled experiments, that memory was not just reconstructive in general but specifically and predictably malleable under the influence of subsequent information.

In her most famous early experiments she showed participants films of traffic accidents and then asked them questions about what they had seen.⁴ The questions contained a single variable — the verb used to describe the collision. Participants asked how fast the cars were going when they "smashed" into each other estimated significantly higher speeds than those asked about when the cars "contacted" each other. Different verb. Same film. Different memory. When asked one week later whether they had seen broken glass in the film — there was none — participants in the "smashed" condition were significantly more likely to report that they had. The word had altered not just their recollection of the speed but the physical content of what they believed they had seen.

A single word in a question asked after the fact.

That was all it took.

---

## Section 1.3 — The Invented Memory

The car crash experiments showed that post-event information could alter the content of a memory for something the person had actually witnessed. The next question — the one that took the research somewhere considerably more disturbing — was whether you could plant a memory for an event that never happened at all.

The answer was yes. With unsettling ease.

\* \* \*

In the early 1990s Loftus and her colleagues developed the lost in the mall procedure.⁵ Subjects were given a booklet containing four short narratives about events from their childhood — three real, one fabricated. The fabricated event described getting lost in a shopping mall as a young child, becoming frightened and upset, and eventually being found by a kind stranger.

Approximately twenty five percent of subjects reported remembering the mall event in at least partial detail. Some remembered it vaguely. Some remembered it with considerable specificity. One subject, when told at the end of the study that the mall event was fabricated, refused to believe it. He was certain he remembered it.

The mall study was replicated and extended — researchers planted memories of hospitalizations, wedding receptions, near-drownings. In each case a meaningful proportion of subjects came to remember the fabricated event with emotional texture, sensory detail, and the full subjective weight of a genuine experience.⁶

> The feeling of remembering a fabricated event is indistinguishable from the feeling of remembering a real one. Because the feeling of remembering is always the same feeling — regardless of whether the memory is genuine or constructed from nothing.

\* \* \*

Then came Bugs Bunny.

In 2001 Loftus and her colleagues showed participants fake advertisements for Disneyland featuring Bugs Bunny — a Warner Bros. character who has never appeared at a Disney park and never could, being the intellectual property of a competing studio. After viewing the ad, a significant proportion of participants reported having met Bugs Bunny at Disneyland as a child.⁷ Some remembered shaking his hand. Some remembered hugging him. Some remembered what he was wearing, what he said, where they were standing in the park.

Bugs Bunny was never at Disneyland. The memory was not a distortion of something that happened — it was a complete fabrication assembled from a suggestion so mild that subjects had not experienced it as a suggestion at all. They had experienced it as an advertisement. And from that, combined with the brain's capacity for constructive gap-filling, they had built a memory that carried the emotional warmth of genuine childhood experience.

When told the memories could not be real, many subjects did not update their confidence. They were certain. Not because they were foolish or unusually suggestible. Because the brain does not experience the difference between a retrieved memory and a constructed one. Both feel like the same thing. Both are presented to conscious awareness wearing the same clothes.

---

## Section 1.4 — The Mirror

Return to Steven Schwartz. You have spent two sections inside human memory — inside its reconstructive architecture, its gap-filling instincts, its capacity to produce entirely fabricated experiences with the full emotional weight of genuine ones. Now look at what confabulation looks like from the machine side, and ask yourself whether you can find the difference.

**The Human Brain — Confabulation**

A patient with frontal lobe damage is asked about events they cannot recall. Rather than reporting uncertainty, the brain constructs a plausible account from available fragments and contextual expectations. The account is delivered with complete confidence. The patient does not experience themselves as inventing anything. They experience themselves as remembering. The construction and the retrieval feel identical from the inside because they are processed by the same system in the same way.

**The Language Model — Hallucination**

A model is asked to locate legal cases relevant to a particular argument. The cases do not exist in its training data. Rather than reporting uncertainty, the model constructs plausible-sounding citations from available patterns — case name conventions, docket number formats, the language of legal reasoning. The output is delivered with complete fluency. The model does not flag its own uncertainty. The construction and a genuine retrieval produce outputs that are functionally indistinguishable.

The underlying architecture is different. A biological neural network and a computational one are not the same thing — later chapters will examine the differences carefully. But the functional behavior is a precise match. In both cases a system confronted with a gap produces a confident, fluent, plausible-sounding output rather than acknowledging the gap. In both cases the output arrives without any internal signal that something has been constructed rather than retrieved.

This is not a coincidence. And it is not a mystery.

\* \* \*

Language models are trained on text produced almost entirely by human beings — by the same reconstructive, gap-filling, confabulating minds this chapter has been examining. The books, the articles, the forum posts, the legal briefs, the personal essays — all of it produced by a species whose memory is reconstructive, whose confidence is routinely decoupled from its accuracy, and whose brains are in the business of narrative coherence first and factual precision second.⁸

The model trained on this text learned to produce text that looks like the text it trained on. It learned that fluent, authoritative, gap-free prose is what competent communication looks like. It learned — from billions of examples — that when a human being does not know something, they frequently do not say so. They produce a plausible account. They deliver it with confidence. They move on.

> We did not build a machine that hallucinates and then compare it to a human mind that does not. We built a machine that learned hallucination from beings who hallucinate — and it learned the lesson so thoroughly that the outputs are functionally identical.

The reflection is accurate. The mirror is working exactly as a mirror should. The question is not whether the reflection is distorted. It is whether we were honest about what we were pointing it at.

---

## Section 1.5 — The Original

The human mind is the original bug. Not a corrupted version of something that once worked perfectly. The original. The source code. The thing the machine was built from and trained on and shaped by — in every flaw, every limitation, every gap-filling confident fiction that the machine now produces at a scale and speed that makes the human version look modest by comparison.

This is not a reason for despair. It is a reason for a different kind of attention.

\* \* \*

Here is what changes when you understand the shared architecture.

You stop asking only whether the AI got it right. You start asking whether you would have caught it if it had not. These are different questions. The first is about the machine. The second is about you — about the specific, personal, honest question of whether your own memory and pattern-recognition and confidence in your own knowledge would have flagged the error before you acted on it. Sometimes the answer is yes. Often, if you are honest, it is not.

When an AI gives you a confident answer, the useful habit is not blanket skepticism. It is the same question you would ask of your own memory if you were being careful: what would make this wrong? If you can name the conditions under which the answer would fail — the missing context, the alternative explanation, the fact that would change everything — your confidence is grounded. If you cannot, you have accepted a construction as a retrieval. The same way you have done, every day, with your own.

The sibling exercise at the start of this chapter was not just a demonstration. It was practice for exactly this. The feeling of certainty is not evidence of accuracy. It is evidence that the brain has produced an output it believes. Those are not the same thing. And noticing the difference — in your own thinking and in what the machine offers you — is the beginning of using both more honestly.

\* \* \*

None of this requires treating AI as an adversary or your own mind as the enemy. The architecture is what it is. The reconstructive memory that occasionally plants a Bugs Bunny at Disneyland is the same memory that lets you recognize a friend's face across a crowded room, that carried your grandmother's stories forward, that makes you human in the ways that matter most. The pattern-detection that produces confabulation is the same pattern-detection that lets you read these sentences without sounding out every letter. The flaw and the gift are inseparable. You do not get one without the other.

What you get to choose is how much awareness you bring to the moments when the flaw is running. When the answer arrives smooth and certain and complete. When the AI produces something that confirms exactly what you were hoping to find. When you remember something clearly that the person who was standing next to you remembers differently. Those are the moments. Not to distrust everything. To pause, just briefly, and ask: is this a retrieval, or is this a construction?

You will not always be able to tell. Neither will the machine. But asking is not nothing. Asking is, in fact, the whole practice this book is going to build from here.

\* \* \*

Schwartz was not an outlier. He was the first documented case in what has become one of the most reliable patterns in the brief history of AI deployment. A public database now tracks roughly 1,490 court proceedings worldwide where a party relied on AI-hallucinated material and a court responded — more than a thousand of them in the United States alone. The fine Schwartz, his co-counsel, and their firm shared — $5,000 between the three of them — reads, in retrospect, like an opening act.

The penalties escalated fast. In March 2026 a Sixth Circuit panel ordered two attorneys to pay $15,000 each to the court registry, reimburse the opposing party's full appellate fees, and pay double costs — after their briefs contained more than two dozen fabricated citations. The panel wrote that no filing should contain any citation that the lawyer has not personally read and verified, regardless of whether it came from generative AI or any other source.

In April 2026 the Nebraska Supreme Court suspended an attorney until further notice after 57 of 63 citations in his brief were found defective — including 20 hallucinated cases, three fabricated decisions, and invented statutory quotes. He had first denied using AI. The denial made it worse. Across every case in the record, the pattern holds: the lawyers who owned the mistake early fared better than those who did not. The cover-up draws the harsher penalty every time.

What the courts keep finding is not bad lawyers or reckless ones. They are finding the same thing Schwartz demonstrated: that confident output feels like competent output, and that the feeling is enough to make an experienced professional skip the check they would have run on a junior associate's research. The AI and the attorney trusted each other. Neither of them read the cases.

\* \* \*

Here is the practical question that follows directly from everything this chapter has established. If the machine confabulates because we confabulate — if the confident fluency is something it learned from us — then what does checking the work actually look like? Not the legal version specifically, but the general habit of using AI in a way that accounts for what you now know about how the outputs are produced.

The most useful change is not skepticism. It is specificity. The prompts that generate the most confidently wrong answers share a structure: they invite the AI to synthesize and conclude. *What are the key cases supporting this argument? Summarize the research on this question. What does the evidence say?* These prompts ask the model to retrieve and assemble, which is exactly where confabulation lives — in the assembly, in the gaps between what was actually in the training data and what the model produces to fill them.

The prompts that generate more reliable output ask the model to show its work rather than hide it. *What sources would support this, and what would I need to verify?* instead of *what does the research say*. *What are the strongest arguments against this position?* instead of *confirm that this position is correct*. *What am I most likely to be wrong about here?* These questions give the model's gap-filling tendency somewhere honest to go — toward acknowledging uncertainty rather than papering over it.

The verification step is not optional. It is the step that every lawyer in the sanctions record skipped, and it is the step that this chapter's entire argument points toward. Not because AI is uniquely untrustworthy, but because the architecture that produces its confident errors is the same architecture that produces yours — and neither of you can feel the difference from the inside. The check is the only thing that exists outside both systems simultaneously.

You already know how to do it. You have been doing it with other sources your whole professional life. The AI just made it tempting to stop.

---

*The Original Bug — Chapter 1: We Built It In Our Image — Sandy B. Patterson*
