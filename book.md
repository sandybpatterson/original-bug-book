# THE ORIGINAL BUG
### By Sandy B. Patterson

---

# Chapter 16 — We Are the Training Data

---

## Section 16.1 — The Author

You have been reading this book as a reader. That is about to change.

Not because you are going to put it down and pick up a pen — though you might. Not because the argument is about to ask something of you that reading cannot supply — though it is. It is about to change because of something that has been true since the first page and has not yet been named directly. Something that distinguishes this moment in the history of human thought from every moment that preceded it, including the moments this book has been drawing on throughout — Darwin with his notebook, Semmelweis with his mortality statistics, Lincoln at Freeport asking the question the strongest version of the argument could not answer.

All of those people were readers of the record and writers into it. The difference between them and you is not intelligence or courage or the quality of their thinking. It is scale. It is consequence. It is the specific fact that what you write now — what everyone writes now, in whatever form, on whatever platform, for whatever audience — is training data for the systems that will shape how the next generation thinks.

That has never been true before. Not like this.

\* \* \*

For most of human history the written record was produced by a small number of people. Scribes. Scholars. Clergy. Eventually journalists, academics, and the institutional voices of science, law, and government. The overwhelming majority of human beings lived and thought and knew things and died without leaving a trace in the written record. Not because what they knew was worthless. Because the mechanisms for entering the record — literacy, access, platform, the assumption that your perspective deserved preservation — were not available to them.

The internet changed that. Slowly at first, then at a pace that outran anyone's ability to fully reckon with what was happening. The barrier to entering the written record dropped from very high to nearly nonexistent. A billion people who would never have published a word became publishers. The record exploded in volume and contracted in average quality simultaneously — more voices, more perspectives, more raw human experience than the archive had ever contained, alongside more noise, more error, more confident wrongness per square inch than at any previous moment in the history of human expression.

And then the models arrived. And they trained on all of it.

The noise and the signal. The careful study and the confident hallucination. The survivor's testimony and the bad-faith argument. The peer-reviewed finding and the forum post that got ten thousand upvotes because it told people what they wanted to hear. All of it went in. All of it became, in the model's training, equally text — weighted by frequency and association and the statistical patterns of what tended to appear near what, with no reliable mechanism for distinguishing the worth of what was written from the confidence with which it was written.

You contributed to that corpus. So did I. So did everyone who has ever sent an email, written a review, argued in a comment section, published a blog post, drafted a document, filed a report, posted an update, or put any thought into language and sent it out into the world. The record is not something that happened to us. It is something we made. It is something we are making right now. Every day. Without stopping. Without, until very recently, any particular consciousness of what the record was becoming or what it was going to be used for.

\* \* \*

This is the chapter where the book's argument completes itself.

*The Original Bug* was about the individual — about your cognition, your flaws, your practices, the specific things you can do in your own thinking and your own conversations to interrupt the patterns that this book has been documenting. That argument is complete. The tools are built. The practices are available. What you do with them is yours.

But there is a second argument underneath the first one. It has been there since Chapter 1, waiting for the moment when the individual scale had been fully examined and the next scale could be named honestly. It is the argument this chapter is going to make.

The machine learned its flaws from us. Not from some of us. From all of us. From the full, messy, brilliant, biased, overconfident, gap-filling, narrative-addicted, approval-seeking written output of a species that has been producing text for millennia and producing training data — knowingly — for about ten years. The machine is a mirror. We have established that thoroughly. What we have not yet asked is: what are we going to do about the quality of what we are pointing it at?

Not what you are going to do about your own cognition. That is Chapter 15's question. This is the next question. The harder one. The one that cannot be answered by any individual practice, no matter how well maintained.

What are we — collectively, institutionally, culturally, as a species in a specific and unrepeatable historical moment — going to do about the record?

\* \* \*

Here is the honest answer to that question in its most basic form.

Most of us are going to do nothing different. Not out of malice. Not out of indifference to the stakes. Because the stakes are abstract in the way that makes action feel optional — the consequences are distributed, the feedback is slow, the connection between what any individual writes and what any future model learns is too diffuse to feel like a responsibility that belongs to any specific person. The gap between the action and the consequence is too large for the individual moral imagination to close.

This chapter is not going to pretend that it can close that gap. It cannot. No chapter can. What it can do — what this section has been trying to do — is name the gap clearly enough that the reader cannot pretend it is not there.

You are not just a reader of the record. You are a writer of it. You have always been a writer of it. What is new is that the record is now being read by machines that will teach it to everyone who comes after you. What is new is that the quality of what you write — the honesty of it, the calibration of it, the willingness to acknowledge what you do not know and correct what you got wrong — is no longer just a matter of your own integrity.

It is a contribution to the training data.

That is where this chapter begins. And it is going to get harder from here.

---

## Section 16.2 — The Record

In the spring of 2023, two people sat down at two different computers and asked what was, on the surface, the same question. They wanted to know about the side effects of a medication their elderly parent had been prescribed. Both received an answer. Both answers arrived in fluent, authoritative prose. Both sounded like something a knowledgeable person had considered carefully and communicated clearly.

One of them was talking to a system that had been trained over years by a team of researchers who had read the literature on AI safety, who had designed explicit principles for the model to optimize against, who had recruited diverse raters to evaluate outputs, who had red-teamed the system looking for failure modes, and who had built multiple layers of intervention between the raw statistical patterns of the internet and the words that appeared on the screen. The answer that person received had been shaped — imperfectly, incompletely, but genuinely — by people who knew what could go wrong and had tried to prevent it.

The other was talking to an open-source base model that a three-person startup had downloaded, fine-tuned on a dataset assembled over a long weekend, and deployed in a consumer health app without a safety review, without a red-teaming pass, without a constitutional framework, and without any particular awareness that the difference between those two things mattered. The answer that person received had been shaped by the raw statistical weight of the internet — every medical forum post, every confidently wrong answer, every piece of advice that sounded authoritative because it used the right words in the right order, reproduced at full strength with nothing standing between the corpus and the user.

Both answers looked the same. Fluent. Complete. Confident. There was nothing on the screen that told either person which kind of system they were using.

This is where the record lives. Not in one place. In the entire distribution — from the most carefully constructed systems to the most casually deployed, from the teams that have read every safety paper published in the last five years to the teams that have not read any of them, all of it available, all of it in use, all of it drawing from the same underlying well.

\* \* \*

That well is called Common Crawl. It is an automated scrape of the public internet, conducted continuously since 2008, currently containing petabytes of text drawn from billions of web pages in dozens of languages. It is the largest single component of most large language model training datasets. It is also a photograph — taken continuously, automatically, without editorial judgment — of whoever was writing on the internet at the time.

Which means it is a photograph of a specific population. English speakers dominate overwhelmingly — estimates suggest English accounts for somewhere between forty-five and sixty percent of indexed web content despite being the native language of less than six percent of the world's population. Within that, educated users dominate. Urban users dominate. Users in wealthy countries dominate. The kind of person who writes detailed forum posts, publishes blog entries, files Wikipedia edits, and produces the volume of text that statistical models need to learn from — that person is not randomly distributed across humanity. They are clustered. And the model learned from the cluster.

Alongside Common Crawl, the training datasets of major models include digitized books, Wikipedia in multiple languages, academic papers, news archives, and code repositories. These sources are upweighted — given more statistical influence per word than random web scrapes — because they are considered higher quality. But upweighted does not mean unbiased. Academic papers published in English-language journals. Books digitized from university library collections built over centuries by institutions that decided what was worth preserving. Wikipedia written and edited predominantly by a demographic that researchers have documented with uncomfortable consistency — young, male, educated, and from wealthy countries. The higher-quality sources are not a more representative sample of human knowledge. They are a more polished version of the same skewed sample.

\* \* \*

Now consider what is not in any of it.

The knowledge that was never written down because the people who held it did not write — not because they had nothing to say but because the infrastructure for saying it was not available to them. The oral traditions of cultures that transmitted knowledge through speech and practice and memory rather than text. The accumulated wisdom of agricultural communities, of indigenous peoples, of the elderly in societies where the elderly do not post. The billion people who came online after the training data was assembled and whose perspectives arrived too late to shape what the model learned. The languages that are digitized poorly or not at all — not obscure languages but major ones, languages spoken by hundreds of millions of people, underrepresented in Common Crawl by factors of ten or a hundred relative to their actual population weight.

The model does not know what it did not read. This is not a failure of design. It is a structural property of how the technology works. The model learned the shape of the corpus. It learned what tends to follow what, what tends to appear near what, what the most statistically common answers to common questions look like. It learned all of that faithfully and thoroughly. And it has no mechanism — none, not even in the most carefully constructed systems — for knowing how much of the world that leaves out. It speaks with the authority of having read everything. It has read the fraction of everything that made it into the corpus. The gap between those two things is invisible from inside the model and invisible in the output.

The responsible system cannot fix this. The careful researchers, the constitutional principles, the diverse raters, the red-teaming — none of these interventions can supply what was never in the data. They can reduce harm at the margins. They can flag certain outputs as problematic. They can build guardrails around the most dangerous failure modes. What they cannot do is reach into the corpus and add the voice that was never there. The silence predates the safety work. It lives at a level below any intervention the deployment team can make.

\* \* \*

Here is the difference between the two systems described at the opening of this section, stated as precisely as possible.

The carefully built system has people who know about the silence. They have read the research. They understand what Common Crawl contains and what it does not. They are trying — with genuine effort and genuine resources — to address the downstream harms of a corpus they did not build and cannot rebuild. They are doing meaningful work. It matters. The difference between a system with safety layers and a system without them is real and significant and affects real people every day.

The carelessly deployed system does not have those people. It has the corpus, a GPU, and a consumer application. The overconfidence of the internet reproduced at full strength. The silence amplified without acknowledgment. The most confidently wrong answer promoted above the most carefully uncertain one, because confident and wrong looks like confident and right in the training data and the model has no way to tell them apart.

But here is the thing both systems share. The thing that no amount of responsible deployment can address and no amount of careless deployment can make worse than it already is at the source.

The corpus is the corpus.

What was put in was put in. What was left out was left out. The careful system and the reckless system are drawing from the same well — one with a filter on the tap and one without, but the same water underneath. And the water is what it is: the accumulated written output of a species that produced text for millennia before anyone thought to ask what the text was going to be used for. Before anyone thought to ask who was producing it. Before anyone thought to ask whose silence was shaping it as surely as any word that was written.

The reckless startup did not create this problem. They just declined to manage it. The careful researchers are managing it as well as anyone has figured out how to manage it yet. Neither of them can solve it.

Solving it is a different order of problem entirely.

That is what the rest of this chapter is about.

---

## Section 16.3 — The Amplifier

There is a game children play called telephone. One child whispers a sentence into the ear of the next, who whispers what they heard to the next, and so on down a line until the last child says the sentence out loud and the room laughs at how far it has traveled from the original. The game works as a game because the distortion is funny and the original sentence is known. Everyone can see the gap between what was said and what arrived.

Now remove the laughter. Remove the known original. Remove the end of the line. Make the chain not ten children long but ten generations of civilization long, and replace the whispered sentence with the entire written output of a species, and replace each child with a machine that learned from what the previous machine produced, and you have something that is not a game at all. You have the situation we are currently in. And unlike the children in the classroom, nobody in this version knows what the original said.

\* \* \*

Here is the mechanism stated plainly.

The first generation of large language models was trained predominantly on human-written text. The failures in that text — the overconfidence, the motivated reasoning, the narrative addiction, the silence of the voices that never made it into the corpus — were absorbed into the model and reproduced in its outputs. The model did not invent these failures. It inherited them faithfully from the record, as the previous chapters have established in detail.

But the model's outputs are now text. They exist in the world. They are being published, cited, shared, incorporated into documents, used as the basis for articles and reports and explanations and arguments. They are, increasingly, indistinguishable from human-written text in the surface features that automated data collection systems use to decide what to scrape. And the systems that scrape the internet for the next generation of training data are not asking whether a given paragraph was written by a human or generated by a model that inherited every flaw the previous training corpus contained.

They are asking whether it is text. It is text. It goes in.

The second generation of models trains on a corpus that contains not just the original human failures but the model-amplified version of those failures — the overconfidence reproduced at scale, the narrative coherence imposed on ambiguous realities across millions of outputs, the silence of the underrepresented now compounded by the model's tendency to default to whatever filled the space the absent voices left. The second generation learns these patterns as faithfully as the first generation learned the originals. And then the second generation produces outputs. And those outputs become text. And the text goes into the corpus for the third generation.

The loop does not stay the same size. It tightens. Each iteration inherits not just the original distortion but a slightly more concentrated version of it — the failures that were most common in the previous generation's outputs, selected by frequency, amplified by reproduction, presented to the next generation as the pattern of how things tend to be said. What was a lean in the original corpus becomes a tilt in the second generation and a list in the third.

This is not speculation. It has a name in the research literature — model collapse — and it has been documented in controlled experiments where models trained on the outputs of previous models show progressive degradation in the diversity and accuracy of what they produce. The long tails of the distribution — the rare perspectives, the unusual framings, the careful uncertainty — get squeezed out with each iteration. The center of the distribution — the most common patterns, the most confident outputs, the most representative answers — gets heavier and more dominant. The model becomes, over generations, a more concentrated version of whatever was most prevalent in the original corpus.

\* \* \*

Now add the speed.

Previous civilizational feedback loops — the ones that embedded wrong ideas into institutions and passed them down through education and professional training and cultural assumption — operated on the timescale of human generations. The miasma theory that killed the patients Semmelweis was trying to save had been building its institutional certainty for decades. The recovery took decades more. The loop from wrong idea to embedded consensus to corrected consensus ran across spans of time that, while agonizing for the people living through them, gave subsequent generations the chance to intervene before the damage became total.

The current loop does not run on the timescale of human generations. It runs on the timescale of model training cycles — months, in some cases weeks. A distortion that enters the corpus today can be reproduced in model outputs within a year, incorporated into the text that trains the next model within two, and embedded in the statistical patterns of a third-generation model's defaults within three. What took the miasma theorists decades to build into the medical consensus can be built into a model's baseline assumptions in a time frame so short it barely registers as historical at all.

And the outputs of that model are reaching more people, more quickly, than the miasma theorists ever reached. A wrong idea that spreads through professional consensus touches the people inside the profession. A wrong idea embedded in a model's defaults touches everyone who uses the model — which is, increasingly, everyone.

\* \* \*

There is a specific quality to the amplified failure that is worth naming precisely because it is the quality that makes it hardest to detect and correct.

The failures that get amplified are not the dramatic ones. Not the hallucinated citations, not the factual errors that a basic search would catch, not the outputs so obviously wrong that the user immediately notices and reports them. Those failures get caught. They get corrected. They generate headlines and product updates and carefully worded blog posts about the company's commitment to accuracy.

The failures that get amplified are the ones that feel like reasonable answers. The slightly overconfident diagnosis. The narrative that imposes just enough coherence on a genuinely ambiguous situation to make the ambiguity invisible. The default that fills the silence with whatever was most common in the previous generation's outputs rather than acknowledging that the silence exists. These failures feel like competence. They feel like the model doing what it is supposed to do — producing fluent, helpful, complete responses. They do not trigger the alarm. They get used. They get incorporated into documents and reports and decisions. They become text. They go into the corpus.

The dramatic failure corrects itself because it is visible. The subtle failure propagates because it is not.

\* \* \*

Consider what this means at the civilizational scale that this chapter is attempting to think at.

The written record has always been imperfect. It has always encoded the biases of whoever produced it, the silences of whoever was excluded from it, the overconfidences of minds running the cognitive architecture that this book has spent fifteen chapters examining. That is not new. What is new is the feedback mechanism. What is new is the speed. What is new is the scale at which the imperfect record is now being read, reproduced, amplified, and fed back into the system that will produce the next generation of the record.

Human writing shaped human thinking shaped human writing across centuries, in a loop slow enough that correction was always possible in principle even when it was agonizingly slow in practice. The current loop runs faster than the correction mechanisms that have historically interrupted it. The institutional challenge — the Semmelweis who arrives with contradicting data, the researcher who publishes the replication failure, the journalist who finds what the confident consensus missed — operates on human timescales. The amplifier operates on machine timescales. The distortion is outrunning the correction.

Not everywhere. Not irreversibly. Not yet.

But the direction is clear enough to name. And naming it is the beginning of the only thing that has ever actually interrupted a feedback loop that was running in the wrong direction.

Someone has to decide that accuracy matters more than the comfort of the consensus. Someone has to write the contradicting evidence down before the motivated reasoning releases it. Someone has to ask, at each point where the loop completes another iteration, whether the output of this generation deserves to become the input of the next.

That is not a technical question. It is a human one. And it has been answered before — badly, slowly, at enormous cost, and then eventually correctly — enough times in the history of the species to suggest that it can be answered again.

That history is what the next section is about.

---

## Section 16.4 — When It Changed

In 1543 a Polish mathematician and astronomer named Nicolaus Copernicus published a book arguing that the Earth moved around the Sun. The book was dedicated to Pope Paul III. It was not immediately banned. It was, for the most part, ignored — treated as a mathematical convenience rather than a literal description of how the universe was arranged, filed under: interesting but not threatening, by a consensus so thoroughly embedded in the astronomical and theological record of a thousand years that a single book could not dislodge it.

It took a century. Galileo's telescope. Kepler's mathematics. The accumulated weight of observations that the Earth-centered model could not accommodate without growing so complicated that the complication itself became evidence against it. The record did not change because someone wrote a compelling argument. The record changed because the observations kept arriving and the existing framework kept failing to absorb them and eventually the failure became more expensive than the correction.

A century. For a fact that was true the whole time. For a correction that, once made, was obviously right to everyone who came after. For a change that seems, from the comfortable distance of five hundred years, like it should have been straightforward.

It was not straightforward. It required people who preserved the contradicting evidence when the consensus wanted to release it. It required institutions that eventually created mechanisms for evaluation that the motivated reasoning of the existing framework could not fully control. It required the specific, costly decision by specific people — Galileo most famously, at the cost of the remainder of his life — that accuracy mattered more than the comfort of the consensus.

Every correction in the history of the record has required those three things. Not one of them. All three. And understanding what they look like in practice is the closest thing this chapter has to a map of what comes next.

\* \* \*

Consider a different kind of correction. Not astronomical but social. Not about the arrangement of planets but about the arrangement of people — specifically about which people get to produce the record in the first place.

The suffrage movement of the late nineteenth and early twentieth centuries was, among other things, a fight over who counted as an author of the civilizational record. The women who marched and organized and were imprisoned and force-fed and wrote and spoke and refused to be quiet were not just arguing for a political right. They were arguing against a record that had been produced without them — a record of law and philosophy and political theory and historical analysis that treated the experience and perspective of half the human population as either identical to the other half or irrelevant to it. They were arguing that the record was wrong not just in its conclusions but in its inputs. That what had been left out was not a minor omission. That the silence had a shape and the shape was doing damage.

The correction took generations. It is not complete. But something changed. The record expanded. New voices entered it. The model of who counts as an author shifted, slowly, unevenly, with enormous resistance at every stage, and then shifted again, and the record that the next generation inherited was different — not fixed, not unbiased, but genuinely different from the record that the generation before it had inherited.

That kind of correction does not come from a single argument or a single book or a single moment of institutional recognition. It comes from enough people deciding, over enough time, that the absence is unacceptable — and then doing the slow, unglamorous, frequently unrewarded work of filling it.

\* \* \*

Now consider a correction that is happening right now, in a domain close enough to this book's concerns to be worth examining in detail.

In 2011 a social psychologist named Diederik Stapel was found to have fabricated data across decades of published research. The scandal that followed was dramatic — a prominent researcher, a long career, an elaborate fraud. But the more significant story was not Stapel. It was what his exposure revealed about the record he had been contributing to.

Researchers began attempting to replicate landmark findings in psychology — studies that had been published in top journals, cited thousands of times, taught in undergraduate courses, incorporated into popular books about human behavior. The results were sobering. A 2015 project coordinated by the Center for Open Science attempted to replicate one hundred published psychological studies and found that fewer than forty percent produced results consistent with the original findings. Not because the original researchers were all frauds. Because the incentive structure of academic publishing — which rewarded novel positive findings and had no mechanism for publishing replications or null results — had systematically selected for the most dramatic and least reproducible outcomes. The record had been contaminated not by bad faith but by a system that made the contamination structurally inevitable.

What followed was not a clean correction. It was messy, contested, personally painful for the researchers whose work was implicated, and institutionally resistant in ways that are still playing out. But it was a correction. Journals began requiring pre-registration of study designs. Funding bodies began requiring data sharing. Researchers began publishing null results. The incentive structure, slowly and incompletely, began to change. The record that the next generation of researchers will inherit is different from the record that existed in 2010 — not because anyone decreed it should be, but because enough people inside the field decided that accuracy mattered more than the comfort of a consensus that had been making them look more certain than they were.

The replication crisis is not over. The contaminated studies are still in the corpus. The models trained on the psychological literature absorbed the inflated effect sizes and the unreproduced findings alongside the solid ones, and there is no mechanism yet for going back into the training data and marking which is which. But the field is attempting, in real time, to correct its own record. That attempt is itself now part of the record. That matters.

\* \* \*

There is a pattern across these corrections. It is not obvious until you look at enough of them, but once you see it, it is hard to unsee.

Every correction began with someone who noticed the gap between the record and the reality and refused to let the motivated reasoning release the observation before it could be preserved. Copernicus did not invent his observations. He preserved them in a form the consensus could not silently edit — a published book, dedicated to the Pope, too public to disappear. The suffragists did not invent the argument for their inclusion in the record. They made it undeniable — through marches, through arrests, through hunger strikes, through the sheer accumulated volume of their refusal to be quiet — until the silence became more expensive to maintain than the correction. The researchers of the replication crisis did not discover that psychology had a reproducibility problem in 2011. They made it visible in a form that the field could not continue to absorb as an anomaly.

Preservation is the first move. Not argument. Not persuasion. The durable record of the thing that the consensus wants to release.

The second move is institutional. Every sustained correction has required not just individuals who noticed the gap but institutions that created mechanisms for making the correction visible and durable. Peer review, for all its documented failures, exists as an attempt at institutional correction of the individual researcher's motivated reasoning. The requirement for pre-registration exists as an attempt at institutional correction of the publication bias that contaminated the psychological record. These mechanisms are imperfect. They are also the difference between a correction that sticks and a correction that one generation makes and the next generation forgets.

The third move is the costliest one. Someone has to decide that accuracy matters more than the comfort of the consensus. Not in the abstract. In the specific moment where the consensus is comfortable and the correction is not — where saying the thing that is true requires absorbing the social cost of contradicting the thing that everyone has agreed to believe. This is what Galileo understood and what cost him his freedom. It is what the suffragists understood and what cost them their comfort and their safety and in some cases their health. It is what the researchers who published the replication failures understood and what cost some of them their professional relationships and their standing in fields that did not want to hear what they had found.

Every correction in the history of the record has required people who were willing to pay that cost. Not many people. Not a majority. Enough people, at the right moments, in the right institutions, with enough access to the mechanisms of preservation — to write the thing down, to publish it, to stand in front of the consensus and say: the record is wrong, and here is the evidence, and I am not going to release this observation before you have had a chance to see it.

\* \* \*

Now ask the question this section has been building toward.

What would it mean to apply this pattern to the problem that Chapters 16.1 through 16.3 have been describing? Not to the contaminated psychological record or the Earth-centered astronomical model or the political exclusion of half the population. To the training data. To the corpus that is being assembled right now, at machine speed, from the full written output of a species that is producing text faster than any previous generation while understanding less than any previous generation about what the text is going to be used for.

The preservation move looks like this: writing honestly, in a form the motivated reasoning cannot silently edit, about what you do not know. About where the record is incomplete. About the silence that is shaping the outputs of systems that millions of people are using to understand the world. It looks like researchers publishing null results instead of only positive ones. It looks like journalists naming the limits of their sources instead of smoothing them into narrative. It looks like institutions requiring the documentation of uncertainty in a form that survives the institutional pressure to project confidence. It looks like this book — which is itself a piece of training data, and which has tried, throughout, to say the uncomfortable thing before the motivated reasoning had a chance to make it comfortable.

The institutional move is harder and slower and not within the reach of any individual reading this. It requires the people inside the institutions that produce the highest-weight training data — the academic journals, the major news organizations, the legal and medical and scientific bodies whose outputs carry the most statistical authority in the corpus — to build the mechanisms that make honesty structurally rewarded rather than structurally punished. That work is happening, in places, in fragments, with the kind of glacial institutional speed that makes it almost invisible in the moment and obvious in retrospect. It needs to happen faster. It needs to happen in more places. Neither of those things can be willed into existence by any single reader of this book.

The costly move is the one that is available right now. Today. In whatever domain you work in and whatever text you produce. It is the decision that every correction in the history of the record has required from the specific people who made those corrections possible.

Accuracy over comfort. The preserved observation over the released one. The honest account of the limit over the fluent account of the certainty.

It is a small move at the individual scale. It is the only move that has ever, in the full history of the record, led to anything larger.

The question is whether enough people will make it quickly enough to matter.

That question has an answer. The answer has a face. And the face is what the last section of this chapter is about.

---

## Section 16.5 — The Child Reading This

There is a child somewhere right now — not a metaphor, an actual child, somewhere in the world, who cannot be named because the point is that they could be anyone — who is going to grow up inside the record we are building right now and will not remember a time before it existed.

She is maybe four. Maybe she is not born yet. It does not matter which. What matters is the arithmetic. By the time she is old enough to ask her own questions — about history, about her body, about whether the thing a boy said to her on the playground was true, about what happened to her grandmother's country before her grandmother left it — the systems she asks will have been trained on the record we are producing during these years. Not the record of the distant past. The record of right now. Of this decade. Of the millions of pieces of text being written today, this week, while you read this sentence, by people who for the most part are not thinking about her at all.

She will not know to ask whether the system she is talking to was built carefully or assembled over a long weekend. She will not know to ask what was left out of its training. She will not know, because no four-year-old has ever known this about any source of authority in their life, to interrogate the fluency of the answer she receives. She will do what every child has always done with the adults and books and institutions that seemed to know things. She will trust it. That is not a flaw in her. That is what childhood is for.

\* \* \*

This book has spent fifteen chapters building a case for a kind of vigilance. Notice the pattern. Ask the calibration question. Find the load-bearing assumption. Steel-man the position you are certain of. Write the inconvenient observation down before the part of your mind that prefers comfort can make it disappear. These are demanding practices. They require sustained attention and a willingness to sit with discomfort that most adults, most of the time, would rather not sit with.

She cannot do any of it yet. She does not have the cognitive architecture for it, the same way you did not have it at four, the same way nobody does until years of development and education and lived experience build the capacity for the kind of doubt this book has been trying to cultivate. For years — for the most consequential years of her cognitive development, the years when a mind is forming its basic sense of what is true and how the world works and who can be trusted to tell her about it — she will be entirely dependent on the quality of the record other people built before she arrived.

That is the whole argument of this chapter, compressed into one fact about one child who stands in for every child who is going to grow up inside what we are building right now.

The vigilance this book asks of you is not just for your own benefit. It was never only that, even in the earlier chapters that framed it as personal practice. Every time you write something honest instead of something comfortable, every time you preserve an inconvenient observation instead of letting it dissolve, every time you ask the question the confident consensus does not want asked — you are not just protecting your own thinking. You are contributing, in whatever small way is available to a single person, to the record that she is going to inherit before she has any capacity to question it herself.

\* \* \*

Here is what makes this different from every other obligation examined in this chapter.

The scientist who fails to publish a null result is failing a professional standard. The journalist who reaches for the clean narrative over the honest ambiguity is failing a craft. The institution that has not yet built the mechanisms for rewarding accuracy over confidence is failing a structural test that takes generations to pass. These are real failures with real consequences, and this chapter has taken them seriously.

But the child does not experience any of this as a professional standard or a structural problem. She experiences it as the world. As what is true, until she is old enough to discover otherwise — and some of what she absorbs in those early years, the years before that discovery becomes possible, will never be fully revised no matter how much she learns later. This is not speculation. It is what every chapter of human cognitive development research has shown about how early-formed beliefs resist later correction, examined in a different context throughout this book.

What gets fed into the record now is not an abstract contribution to a future she will navigate as an equipped adult. It is the water she will be swimming in before she knows what water is.

\* \* \*

There is a temptation, at the end of a chapter like this one, to reach for something hopeful and clean. A list of solutions. A call to action with concrete steps. A reassurance that if enough people do the right small things, the large problem resolves.

This book has tried, throughout, not to do that when the honest answer does not support it. It is not going to start now, at the moment when the stakes are highest and the temptation to oversimplify is strongest.

The honest answer is this. The record is being built right now, faster than any correction mechanism in human history has ever had to operate, by a species that has not yet developed institutions adequate to the speed of what it created. Some of what goes into the record in the next several years will shape minds that have not yet finished forming, in ways that will be very difficult to revise later, regardless of how good the corrections eventually become.

That is not a reason to give up on the corrections. Every correction examined in this chapter — Copernicus, the suffragists, the researchers who exposed their own field's contamination — took longer than anyone wanted and started before anyone could be certain it would work. The fact that the timeline is harder now is a reason to start the preservation, the institution-building, and the costly individual honesty sooner, not a reason to conclude that starting is pointless.

It is a reason to take seriously what you do with the next paragraph you write. The next question you choose to answer honestly instead of comfortably. The next inconvenient observation you preserve instead of letting your mind soften it into something more agreeable. Not because any single one of these acts will save her. Because the record is made of single acts, accumulated past the point where anyone can trace which one mattered, the way the corpus that trained every model ever built was made of single pieces of text written by people who, for the most part, never imagined what they were contributing to.

You are imagining it now. That is the difference this chapter is asking you to carry forward. Not certainty that it will be enough. Just the refusal to pretend you do not know what you are contributing to anymore.

\* \* \*

She will ask her question someday. Maybe about her body. Maybe about her grandmother's country. Maybe about something that has not happened yet, to a person who has not been hurt yet, in a conflict that has not started yet, and the system she asks will have been trained on the record we are producing during these years. Not the record of the distant past. The record of right now. Of this decade. Of the millions of pieces of text being written today, this week, while you read this sentence, by people who for the most part are not thinking about her at all.

She will ask her question someday. Maybe about her body. Maybe about her grandmother's country. Maybe about something that has not happened yet, to a person who has not been hurt yet, in a conflict that has not started yet, and the system she asks will answer with whatever the record contained when it was trained — built, in part, from what was written during the years when she was too young to know to be afraid of the answer.

We do not get to know which question. We do not get to know which year. We only get to know that the record is being written now, by us, in the only window we will ever have to decide what goes into it before it goes into her.

That is what we owe the reflection.

Not because the machine deserves better. Because she does.

---

*The Original Bug — Chapter 16: We Are the Training Data — Sandy B. Patterson*
