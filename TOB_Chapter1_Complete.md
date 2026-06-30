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

They treated confabulation as a flaw the machine had developed — something introduced in the engineering, something that distinguished the AI's unreliability from human reliability. They positioned the lesson as: the machine does this, so check the machine's work. What they did not examine was the prior question. Why does the machine do this? Where did it learn to? What, exactly, was it trained on — and what does the content of that training tell us about the nature of the flaw?

The training data that produced these models was generated almost entirely by human minds. Books written by humans. Articles written by humans. Legal briefs written by humans. Scientific papers, Wikipedia edits, forum posts, social media arguments — all of it produced by a species whose memory is reconstructive, whose confidence is routinely decoupled from its accuracy, and whose brains are in the business of gap-filling first and factual precision second.

We did not build a machine that confabulates and then compare it to a human mind that does not.

We built a machine that learned confabulation from beings who confabulate — and it learned the lesson completely.

The question this book is going to keep asking — in every chapter, across every flaw we have identified in artificial intelligence — is not whether the machine is broken. It is whether we have ever been honest about the condition of the original. About the mind the machine learned everything it knows from. About what was already in the training data long before the first model was ever trained.

That is what this book is about.

And it starts — as all honest examinations do — with looking in the mirror.

---

## Section 1.2 — You Do This Too

Before this chapter goes any further, there is something you need to do. Not for the sake of illustration. Because what comes next will land differently if you have tried it first.

Think of a memory from your childhood. Something specific — a family event, a holiday, a moment with a sibling or a parent that you have carried with you and recalled more than once. Hold the memory in your mind. Notice how it feels. Notice the texture of it — where you were standing, what the light was like, what was said, how it ended. Notice how certain it feels. How real.

**An Exercise Before Reading Further**

If you have a sibling, think of one shared childhood memory you have discussed with them at some point in your life. A birthday. A family trip. A fight. A moment at a parent's expense you both found funny. A day something went wrong or unexpectedly right. Something you were both present for.

Now ask yourself: do you and your sibling remember it the same way? Not roughly the same way. The same way. The same details. The same sequence. The same emotional register. The same account of who said what and who did what and what it meant.

If you have ever actually compared notes with a sibling about a shared memory in any detail, you already know the answer. You do not remember it the same way. You may not even remember the same event. One of you remembers a vacation where something wonderful happened. The other remembers the same vacation and the wonderful thing is not there at all — or it happened differently, or someone else was involved, or it happened on a different day than the one you are both sure about. You were in the same place at the same time. You have completely different memories of it.

This is not because one of you is lying. It is not because one of you has a better memory than the other. It is because memory is not a recording that two people make simultaneously of the same event and store in separate but identical files. Memory is a reconstruction — assembled from fragments, shaped by emotion and attention and prior experience, filled in at the gaps by whatever the brain finds most plausible given everything else it knows. Two people who experienced the same event will reconstruct it differently, because their brains were attending to different things, carrying different contexts, and filling in the gaps with different material. Both reconstructions feel completely real. Both are, in important ways, partly invented.²

> Memory is not a recording. It is a reconstruction — assembled from fragments, shaped by emotion and attention, filled in at the gaps by whatever the brain finds most plausible. Both siblings' versions feel completely real. Both are, in important ways, partly invented.

\* \* \*

The sibling example is useful precisely because it is so ordinary. It does not require a laboratory or an experiment or a controlled condition. It requires only two people who grew up in the same house and have at some point compared notes. The divergence happens not because memory is occasionally unreliable under extreme conditions — stress, trauma, the passage of decades — but because memory is always reconstructive under all conditions. The divergence between siblings is the normal operation of the system, not a failure of it.

Research on sibling memory confirms this with a consistency that should be more unsettling than it is. Studies examining pairs of siblings recalling shared childhood experiences find not just minor discrepancies in detail but substantive disagreements about whether events occurred at all, who was present, what the emotional valence of the experience was, and what it meant. In one particularly striking line of research, siblings presented with each other's accounts of shared memories often rejected the other version not as a different perspective on the same event but as simply wrong — as a memory of something that did not happen. Both were certain. Both were sincere. Both were, in some meaningful sense, right about what they remembered and wrong about what happened.³

The brain does not experience the reconstruction happening. It does not flag the gaps it is filling or the plausible content it is inserting. It produces the output — the memory, complete and vivid and emotionally coherent — and presents it to conscious awareness as a retrieved record. You do not feel yourself constructing the memory. You feel yourself remembering it. The difference between those two experiences is invisible from the inside. It has always been invisible. And that invisibility is not a bug in the system. It is an architectural feature of how human memory works.

\* \* \*

Elizabeth Loftus spent her career making this visible in ways that could not be dismissed. Her approach was methodical, cumulative, and — for the legal system and the scientific establishment alike — deeply uncomfortable. Starting in the 1970s she began demonstrating, through controlled experiments, that memory was not just reconstructive in general but specifically and predictably malleable under the influence of subsequent information.

In her most famous early experiments she showed participants films of traffic accidents and then asked them questions about what they had seen.⁴ The questions contained a single variable — the verb used to describe the collision. Participants asked how fast the cars were going when they "smashed" into each other estimated significantly higher speeds than those asked about when the cars "contacted" each other. Different verb. Same film. Different memory. Not a different description of the same memory — a different memory. When asked one week later whether they had seen broken glass in the film — there was none — participants in the "smashed" condition were significantly more likely to report that they had. The word had altered not just their recollection of the speed but the physical content of what they believed they had seen.

A single word in a question asked after the fact.

That was all it took.

\* \* \*

You have been doing this your whole life. Not occasionally, in dramatic situations, when something important was at stake. Continuously. Automatically. In every story you have ever told about something that happened to you, every argument you have had about what was actually said, every certainty you have carried about how something went. The memory felt solid. It felt like a retrieval. It was a construction — assembled from genuine fragments and plausible inventions, presented to you as a unified whole with no visible seams.

Your sibling remembers it differently not because they have a worse memory than you. Because they built a different construction from the same event. And because neither of you has access to the event itself anymore — only to the constructions you each made of it, and the reconstructions of those constructions you have been making every time you recalled it since.

This is the condition of the original. This is the mind that produced the training data. This is what the machine learned from — not from a record of what happened, but from a species' record of what it remembered happening, which is a substantially different thing, filtered through decades of reconstruction, reconstruction of reconstruction, and gap-filling all the way down.

The machine confabulates because its teachers confabulate.

Its teachers confabulate because that is what teachers do.

Every single one of us. Every single day. Without knowing it is happening at all.

---

## Section 1.3 — The Invented Memory

What the car crash experiments established is troubling enough. A single word in a question asked after the fact can alter what a person believes they saw. The memory itself changes — not just the reported version of it, but the underlying recollection. Post-event information gets woven into the original experience and the two become indistinguishable. You cannot feel the seam from the inside. There is no seam from the inside. There is only the memory, whole and vivid and certain, carrying its invented details as naturally as it carries the genuine ones.

But Loftus did not stop at details. The car crash experiments showed that post-event information could alter the content of a memory for an event the person had actually witnessed. The next question — the one that took the research somewhere considerably more disturbing — was whether you could plant a memory for an event that never happened at all.

The answer, it turned out, was yes. With unsettling ease.

\* \* \*

In the early 1990s Loftus and her colleagues developed a technique they called the lost in the mall procedure.⁵ Subjects were given a booklet containing four short narratives about events from their childhood — accounts assembled with the help of family members who confirmed which events had actually occurred. Three of the narratives described real events. The fourth described something that had never happened: getting lost in a shopping mall as a young child, becoming frightened and upset, and eventually being found and reunited with the family by a kind stranger.

Subjects were asked to read each narrative, try to remember the event it described, and write down whatever details came to mind.

Approximately twenty five percent of subjects reported remembering the mall event — the one that had never occurred — in at least partial detail. Some remembered it vaguely. Some remembered it with considerable specificity. One subject, when told at the end of the study that the mall event was fabricated, refused to believe it. He was certain he remembered it. The feeling of remembering was indistinguishable from the feeling of remembering something real because the feeling of remembering is always the same feeling, regardless of whether the memory is genuine or constructed.

The mall study was replicated and extended. Researchers planted memories of being hospitalized overnight as a child, of attending a wedding reception where someone knocked over a punch bowl, of nearly drowning before being rescued by a lifeguard. In each case a meaningful proportion of subjects came to remember the fabricated event — not as a vague impression but as a memory with emotional texture, sensory detail, and the full subjective weight of a genuine experience.⁶

> The feeling of remembering a fabricated event is indistinguishable from the feeling of remembering a real one. Because the feeling of remembering is always the same feeling — regardless of whether the memory is genuine or constructed from nothing.

\* \* \*

Then came Bugs Bunny.

In 2001 Loftus and her colleagues ran a study in which participants were shown fake advertisements for Disneyland that featured Bugs Bunny — a Warner Bros. character who has never appeared at a Disney park and never could, being the intellectual property of a competing studio. After viewing the ad, a significant proportion of participants reported having met Bugs Bunny at Disneyland as a child. Some remembered shaking his hand. Some remembered hugging him. Some remembered specific details about the encounter — what he was wearing, what he said, where they were standing in the park.⁷

Bugs Bunny was never at Disneyland. He could not have been there. The memory was not a distortion of something that happened — it was a complete fabrication, assembled from a suggestion so mild that subjects had not experienced it as a suggestion at all. They had experienced it as an advertisement. And from that advertisement, combined with the brain's enormous capacity for constructive gap-filling, they had built a memory so real it carried the emotional warmth of genuine childhood experience.

When told the memories could not be real, many subjects did not update their confidence. They were certain. The certainty was not the product of accuracy. It was the product of a brain that does not experience the difference between a retrieved memory and a constructed one — because from the brain's perspective, there is no difference. Both arrive through the same process. Both feel like the same thing. Both are presented to conscious awareness wearing the same clothes.

\* \* \*

Here is what this means, stated plainly and without softening.

Your memory is not a record. It is a story your brain tells you about the past, assembled from genuine fragments and invented connective tissue, revised every time you recall it, and presented to you as fact with no indication of which parts were retrieved and which parts were built. You have memories that feel completely real that are partly or entirely fabricated. You cannot identify which ones they are. Nobody can. Not with introspection, not with confidence, not with the most sincere effort to be honest about what you actually remember versus what you think you remember versus what you have been told happened and incorporated into memory as experience.

This is not a flaw that afflicts some people some of the time. It is the architecture of human memory operating normally under all conditions for every person who has ever lived. The people in Loftus's studies were not suggestible in any unusual way. They were not psychologically vulnerable or cognitively impaired. They were ordinary adults with ordinary memories doing what ordinary memories do — constructing the past from available materials, filling gaps with plausible content, and producing the result as recalled experience with the full conviction of something genuinely witnessed.

They were, in the precise clinical sense of the word, confabulating.

They were doing what Steven Schwartz's AI did in the federal courthouse in New York.

They were doing what you do.

They were doing what every human mind does, every day, across every memory it holds, without a single moment of awareness that it is doing it at all.

The question is what this means for a machine that learned everything it knows from the written output of minds like these. That is the question the next section is going to answer.

---

## Section 1.4 — The Mirror

Return to Steven Schwartz. Return to the brief, the citations, the federal courthouse, the moment when the cases that had seemed so real turned out to have never existed. You have more context now than you did in section 1.1. You have spent two sections inside human memory — inside its reconstructive architecture, its gap-filling instincts, its capacity to produce entirely fabricated experiences with the full emotional weight of genuine ones. You know what confabulation looks like from the human side. Now look at what it looks like from the machine side, and ask yourself whether you can find the difference.

**The Human Brain — Confabulation**

A patient with frontal lobe damage is asked about events they cannot recall. Rather than reporting uncertainty, the brain constructs a plausible account from available fragments and contextual expectations. The account is delivered with complete confidence. The patient does not experience themselves as inventing anything. They experience themselves as remembering. The construction and the retrieval feel identical from the inside because they are processed by the same system in the same way.

**The Language Model — Hallucination**

A model is asked to locate legal cases relevant to a particular argument. The cases do not exist in its training data. Rather than reporting uncertainty, the model constructs plausible-sounding citations from available patterns — case name conventions, docket number formats, the language of legal reasoning. The output is delivered with complete fluency. The model does not flag its own uncertainty. The construction and a genuine retrieval produce outputs that are functionally indistinguishable.

The underlying architecture is different. A biological neural network and a computational one are not the same thing and the differences are real and significant and worth understanding — later chapters will examine them carefully. But the functional behavior — the output behavior, the behavior that matters to anyone on the receiving end — is a precise match. In both cases a system confronted with a gap produces a confident, fluent, plausible-sounding output rather than acknowledging the gap. In both cases the output arrives without any internal signal that something has been constructed rather than retrieved. In both cases the person receiving the output has no reliable way of knowing, from the output alone, whether it is genuine or invented.

This is not a coincidence. And it is not a mystery.

\* \* \*

Language models are trained on text. Specifically, on an enormous corpus of text produced almost entirely by human beings — by the same reconstructive, gap-filling, confabulating minds whose workings sections 1.2 and 1.3 have been examining. The books in the training data were written by humans. The articles were written by humans. The forum posts, the Wikipedia edits, the legal briefs, the scientific papers, the personal essays — all of it produced by a species whose memory is reconstructive, whose confidence is routinely decoupled from its accuracy, and whose brains are in the business of narrative coherence first and factual precision second.⁸

What does text produced by confabulating minds look like? It looks confident. It fills gaps. It produces coherent narratives from incomplete information. It presents reconstructed accounts as direct reports. It does not reliably flag its own uncertainty because the minds that produced it do not reliably experience their own uncertainty — the confabulating brain does not know it is confabulating, and therefore the text it produces does not say so.

The model trained on this text learned to produce text that looks like the text it trained on. It learned the patterns of how confident communication works in human writing. It learned that fluent, authoritative, gap-free prose is what competent communication looks like. It learned — from billions of examples — that when a human being does not know something, they frequently do not say so. They produce a plausible account. They deliver it with confidence. They move on.

The model learned this lesson from a corpus of billions of documents.

It learned it completely.

It learned it so well that the output it produces is indistinguishable, in its confidence and its fluency and its willingness to fill gaps with invented content, from the output of the minds it learned from.

> We did not build a machine that hallucinates and then compare it to a human mind that does not. We built a machine that learned hallucination from beings who hallucinate — and it learned the lesson so thoroughly that the outputs are functionally identical.

\* \* \*

There is a version of the Schwartz story that the technology industry finds comfortable. In that version the hallucination is a known limitation of current models — a technical problem that better training, better retrieval systems, and better grounding techniques will eventually solve. The machine is imperfect. The engineers are working on it. The users should exercise appropriate caution in the meantime. Lesson learned. Moving on.

That version is not wrong. The hallucination problem is real and the engineering work to address it is real and the caution is genuinely warranted. But it is incomplete in a specific and important way. It treats the problem as originating in the machine — as something introduced by the architecture or the training process that could in principle be removed if we were clever enough about how we built the thing. It does not ask where the pattern came from in the first place. It does not ask why a system trained on human text would learn to fill gaps confidently rather than to acknowledge them honestly.

The answer is that the system trained on human text learned to behave the way humans behave. And humans, as section 1.3 established, do not experience the gaps they are filling as gaps. They experience them as memories. As knowledge. As facts they know. The text they produce reflects this — it is written with the confidence of a species that has never had reliable access to the difference between what it remembers and what it has constructed.

That is what went into the training data.

That is what came out of the model.

The reflection is accurate. The mirror is working exactly as a mirror should work. The question — the one this book will keep returning to across every chapter that follows — is not whether the reflection is distorted. It is whether we were honest about what we were pointing it at.

---

## Section 1.5 — The Original

There is a version of the conversation about artificial intelligence that goes like this. The machine is powerful but unreliable. It hallucinates. It confabulates. It produces confident fictions and presents them as facts. We need to be careful with it. We need to verify its outputs. We need to remember that it is not human — that it lacks the judgment, the experience, the common sense that would make it truly trustworthy.

That conversation is happening everywhere right now. In boardrooms and classrooms and congressional hearings and newspaper columns and technology podcasts and dinner tables. It is a reasonable conversation. The concerns it raises are legitimate. The caution it recommends is warranted.

And it is missing something so fundamental that getting it wrong changes the nature of everything that follows.

\* \* \*

The missing thing is this: the comparison being made in that conversation — between an unreliable machine and a reliable human mind — is not a comparison between two things that actually exist. The reliable human mind is not a thing that exists. It has never existed. It will not exist. The human mind is reconstructive, gap-filling, confabulating, confidence-decoupled-from-accuracy, narrative-first and factual-precision-second. This is not a description of minds that are damaged or untrained or operating under stress. This is a description of the normal operation of every human mind that has ever lived, including the most rigorous scientific thinkers, the most careful legal scholars, the most disciplined empiricists the species has produced.

Loftus herself — the researcher who spent her career documenting the fallibility of memory — has publicly acknowledged that her own memory is subject to the same reconstructive processes she spent decades studying. The knowledge of the mechanism does not make you immune to it. The awareness that memory is constructive does not give you reliable access to which parts of your memories are constructed. It gives you humility. It gives you caution. It does not give you a recording where everyone else has a reconstruction.

The human mind is the original bug. Not a corrupted version of something that once worked perfectly. The original. The source code. The thing the machine was built from and trained on and shaped by — in every flaw, every limitation, every gap-filling confident fiction that the machine now produces at a scale and speed that makes the human version look modest by comparison.

> The human mind is the original bug. Not a corrupted version of something that once worked perfectly. The original. The source code. The thing the machine was built from, trained on, and shaped by — in every flaw, every limitation, every gap-filling confident fiction it now produces at scale.

\* \* \*

This is not an argument for despair. It is not an argument that human cognition is worthless or that truth is unattainable or that we should stop trying to think carefully and verify rigorously and build better systems. All of those things remain worth doing — more worth doing, if anything, once you understand what you are working with.

It is an argument for honesty. For the specific, uncomfortable, productive kind of honesty that requires looking at the condition of the original before diagnosing the problem with the copy. Before we ask why the machine confabulates, we should understand that confabulation is a feature of the minds that produced its training data. Before we ask why the machine is overconfident, we should understand that overconfidence is a structural property of human communication that the machine learned from billions of examples. Before we ask why the machine has biases, we should understand that the biases were already in the text — placed there by the people who wrote the text, living in the societies that shaped the people, across the centuries of history that shaped the societies.

The machine is a mirror. It reflects what it was built from. And the reflection is, in the ways that matter most, accurate.

\* \* \*

Here is what the rest of this book is going to do. Chapter by chapter it is going to examine the flaws that have been identified in artificial intelligence — the hallucination, the overconfidence, the pattern obsession, the bias, the narrative dependency, the sycophancy, the shortcut-taking, the failure of genuine understanding — and it is going to make the same argument each time. That the flaw in the machine has a precise counterpart in human cognition. That the counterpart is not a coincidence. That the training data connects them. That the machine learned each flaw from the minds that produced the text it trained on — minds running the same architecture, shaped by the same evolutionary history, producing the same patterns of error at the human scale that the machine now produces at the machine scale.

This is not a comfortable argument. It requires sitting with the recognition that the flaws you are most concerned about in artificial intelligence are also, in important ways, your flaws. That the gap you are trying to maintain between the unreliable machine and the reliable human mind is narrower than the current conversation assumes. That the most urgent question about AI is not only how to make the machine more honest — though that question matters enormously — but whether we are willing to be more honest about the original.

Steven Schwartz submitted a brief full of cases that did not exist. The AI that helped him write it had learned to fill gaps confidently from the written output of a species that fills gaps confidently. The species did not notice it was doing this. The machine did not notice either. The brief went to the court. The judge asked for the cases. There were none.

This is the beginning of an honest accounting of how that happened.

Not just in a federal courthouse in New York.

Everywhere.

Every day.

In every mind that has ever been certain of something it constructed.

Which is every mind that has ever existed.

Including yours.

---

*The Original Bug — Chapter 1: We Built It In Our Image — Sandy B. Patterson*
