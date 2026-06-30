# THE ORIGINAL BUG
### Chapter 8 — The Bias Mirror

---

## Section 8.1 — The Autocomplete

Pick up your phone. Open a text message or an email and start typing a sentence. Before you finish it, look at the suggestions appearing above the keyboard. Three words, offered to you as continuations. You have seen them thousands of times. You probably accept them regularly without thinking about it. They feel like a convenience — a small shortcut, a minor efficiency.

They are a mirror.

Those suggestions come from statistical models trained on text produced by human beings. The model learned, from an enormous corpus of real human communication, which words tend to follow which other words, in which contexts, under which conditions. It learned the patterns of how people write. And the patterns of how people write carry, embedded in their structure, every assumption, every default, every bias that shaped the writing in the first place. The suggestion is not neutral. It is a compressed reflection of what the people who produced the training data tended to say — which is to say, of what they tended to think.

This is the chapter about what got compressed in that reflection. And how much of it should make you uncomfortable.

\* \* \*

In 2017 a team of researchers at Princeton and the University of Bath published a study in the journal *Science* that used a method they called the Word Embedding Association Test — WEAT — to measure bias in word embedding models, the foundational technology underlying most language AI.¹ Word embeddings represent words as points in a mathematical space, arranged so that words with similar meanings or associations cluster together. The closer two words are in that space, the more strongly the model associates them.

What the researchers found was this. Flowers were more strongly associated with pleasant concepts — joy, love, peace — than insects were. That is unsurprising and probably harmless. But the same mathematical structure that associated flowers with pleasant concepts also associated European American names more strongly with pleasant concepts than African American names. Male terms more strongly with career and science. Female terms more strongly with family and arts.

The associations were not programmed. Nobody wrote a line of code that said: associate these names with these qualities. The associations emerged from the training data — from the statistical patterns in the text the model had learned from — which reflected the statistical patterns in how human beings, in the society that produced that text, wrote and thought about these things. The bias was not introduced into the model. It was inherited from the source.

> The bias was not introduced into the model. It was inherited from the source. The training data did not contain explicit prejudice. It contained the accumulated statistical residue of a society that practiced it.

\* \* \*

This matters beyond the academic context of a research paper. Word embedding technology is not a curiosity. It is the foundation on which virtually every modern language AI system is built — including the autocomplete on your phone, the search suggestions in your browser, the content recommendation algorithms deciding what you see next, and the large language models this book has been examining throughout. The WEAT findings are not describing a flaw in one obscure research model. They are describing a structural property of how language AI learns, which means they are describing a property of the systems billions of people interact with every day.

The training data did not contain explicit prejudice. It contained the accumulated statistical residue of a society that practiced it — in its hiring, in its publishing, in its media, in its language, in the words that tended to appear near other words across millions of documents produced across decades of unequal history. The model learned the residue. It encoded the residue. And now it reproduces the residue, at scale, in the outputs it generates, in the suggestions it offers, in the defaults it reaches for when no one has told it what to do.

The autocomplete is not suggesting those words by accident. It is suggesting the words that followed those words in the world that produced it. And the world that produced it was this one.

---

## Section 8.2 — Three Flavors of Bias

Bias in AI is not one thing. It is a family of related problems that share a common origin — human output — but travel different paths from that origin into the systems that inherit them. Understanding the differences matters because the solutions, to the extent solutions exist, are different for each. And recognizing which flavor you are looking at when you encounter a biased output is the first step toward knowing what to do about it.

Three types are worth understanding in depth. They overlap, they interact, and they compound each other in ways that make the combined effect considerably larger than any one of them alone.

\* \* \*

**Historical Bias**

The first type does not require anyone to have done anything wrong in the making of the model. It requires only that the world that produced the training data was unequal — which the world always has been and continues to be.

Consider medical AI. Models trained to assist with diagnosis, treatment recommendation, or risk assessment are trained on clinical data — patient records, trial results, imaging datasets, outcome studies. That data reflects the patients who were studied, the trials that were run, and the populations that were represented in the research literature. For most of the history of modern medicine, clinical research systematically underrepresented women and non-white patients.² The landmark clinical trials that established standard treatment protocols for heart disease, for example, were conducted predominantly on white men. The models trained on that data learned what heart disease looks like in white men. When deployed on populations that were not in the training data, their accuracy drops — not because the model was programmed with any discriminatory intent, but because the history it learned from was discriminatory in its own right.

This is historical bias. The injustice is in the past. The model carries it forward into the present. Nobody building the model introduced it. The only honest responses are to acknowledge it, to supplement training data with more representative samples where possible, and to be explicit with users about the populations on which the model was validated and those on which it was not.

\* \* \*

**Representation Bias**

The second type is about who gets to produce the text that trains the models in the first place. The large language models most people interact with were trained primarily on internet text — web pages, digitized books, forum posts, news articles, Wikipedia. That corpus is vast. It is also not representative of humanity.³ English language content dominates overwhelmingly. Content produced by educated, urban, English-speaking populations in wealthy countries dominates within that. The perspectives, concerns, cultural references, and assumptions embedded in that text are the perspectives of a specific slice of humanity that has disproportionate access to writing, publishing, and being online.

> The model's understanding of the world reflects the understanding of the people who produced the most text. That distribution is not the world. It is a particular, demographically skewed sample of the world's written output.

\* \* \*

**Confirmation Bias in Training**

The third type is the most intimate, because it lives not in the historical record or in the demographics of internet users but in the structure of human reasoning itself — and this book has been examining that structure since Chapter 1.

The feedback mechanisms used to train language models involve human evaluators rating outputs as better or worse, more or less helpful, more or less aligned with what was wanted. Those evaluators are people. People have the confirmation bias documented in Chapter 11, the motivated reasoning, the representativeness heuristic, the social approval dynamics. They rate outputs that fit their expectations as better. They rate outputs that challenge their defaults as worse. Those ratings shape what the model learns to produce. And the result is a model that has been fine-tuned, through the aggregated preferences of human evaluators, toward outputs that fit human expectations — including the biased expectations, the default assumptions, the unreflective patterns that nobody examined because nobody noticed they were there.

The bias enters not in the training data but in the feedback. Not in what the model learned from but in what it was rewarded for. Three entry points. One source: the humans who wrote, rated, and shaped everything the model became.

---

## Section 8.3 — The Cases

Theory is one thing. What follows is what it looks like when the theory becomes a résumé rejected, a photograph mislabeled, a sentence handed down by an algorithm. These are not hypothetical scenarios. They are documented cases — real systems, real outputs, real consequences — that illustrate what happens when the three types of bias described in Section 8.2 leave the research paper and enter the world. Each one is different in domain and in the specific mechanism of failure. Each one is identical in the essential thing: the system did exactly what it was designed to do, and what it was designed to do was trained on a world that was not equal.

\* \* \*

**Case One — Amazon's Recruiting Tool — Historical Bias**

In 2014 Amazon began developing an AI tool to automate the early stages of recruiting — screening resumes, identifying promising candidates, filtering the volume of applications down to a manageable shortlist for human review. The model was trained on ten years of Amazon's own hiring data. Ten years of resumes submitted to Amazon, and ten years of decisions about which candidates were hired, promoted, and evaluated as successful.

The model learned from that history. And that history — like the history of most technology companies over the preceding decade — was predominantly male. The people who had been hired, the people who had been promoted, the people whose career trajectories the model used as its measure of success: they were, in large and statistically significant proportion, men. The model did not learn to value men over women as a deliberate choice. It learned that successful Amazon employees, as defined by the data it was given, looked a certain way. And when it processed new resumes, it downrated candidates whose applications contained signals associated with women — the word "women's" in a phrase like "women's chess club captain," attendance at all-female colleges, certain other markers that correlated, in the training data, with the candidates who had not been hired or had not advanced.⁴

Amazon scrapped the tool in 2018. The engineers who built it had not set out to discriminate against women. They had set out to learn from success. The definition of success they were given was a decade of decisions made in an industry with a documented gender problem. The model learned the lesson its teachers taught it. The lesson was wrong. And it would have been wrong whether or not anyone noticed, because the wrongness was not in the code. It was in the history the code learned from.

\* \* \*

**Case Two — Google Photos — Representation Bias**

In the summer of 2015, a software developer named Jacky Alciné opened Google Photos on his phone and found that the application's automatic image labeling feature had categorized photos of himself and a friend — both Black — under the label "gorillas." The story spread quickly. Google apologized immediately and removed the gorilla label from the application's classification system entirely — a fix that was, in the bluntest possible terms, a workaround rather than a solution.⁵

Removing the label did not address the underlying problem. The underlying problem was that the image recognition model had been trained on a dataset in which dark-skinned faces were dramatically underrepresented relative to light-skinned faces. The model had not learned to see Black faces with the same accuracy and nuance it had learned to see white ones. The representation in the training data reflected the representation in the world of people who had produced and uploaded the photographs the dataset was built from — a world in which access to digital photography, internet connection, and image sharing platforms had not been distributed equally.

The harm was real. The mechanism was impersonal. The model had no intent. It had a training distribution. And the training distribution was the world as it had been, not the world as it should be.

\* \* \*

**Case Three — COMPAS — Confirmation Bias and Historical Bias Combined**

COMPAS — Correctional Offender Management Profiling for Alternative Sanctions — appears in this book for the second time, having appeared in Chapter 4 in the context of heuristics. It returns here because the criminal justice context illustrates the compounding of bias types with particular clarity. The algorithm was trained on criminal justice data. That data encoded decades of racially disparate policing, prosecution, and sentencing. The model learned from that history and reproduced its patterns — assigning higher risk scores to Black defendants at rates that, when examined by ProPublica's 2016 investigation, showed Black defendants were nearly twice as likely as white defendants to be falsely flagged as high risk.⁶

The algorithm was doing what pattern-matching systems do: producing the most representative score for defendants who fit certain profiles. Those profiles were derived from historical data. The historical data was the product of a criminal justice system operating in a society with a documented racial disparity problem. The compounding of historical bias and representation bias produced outputs that were dressed in the apparent objectivity of a numerical score and used to make decisions about human liberty.

None of the three systems described in this section were built by people who wanted to discriminate. All three discriminated. The mechanism was not malice. It was inheritance.

---

## Section 8.4 — The Cultural Default

The three cases in Section 8.3 are documented, specific, and in each instance the harm was visible enough to generate headlines, investigations, and public accountability. They are important precisely because they are concrete — they give the abstract argument a body, a face, a courtroom, a rejected résumé. But they represent the detectable end of a much larger and mostly invisible phenomenon.

The cases that make the news are the ones where the bias produced an output dramatic enough to be noticed. The bias that does not make the news is the bias embedded in the defaults — in the baseline assumptions the model carries into every interaction, in the pictures it paints when nobody has told it what to paint, in who appears in the story it generates when you have not specified who the story is about. This bias is quieter, more pervasive, and in some ways more consequential than the headline cases, because it operates at the level of what feels normal rather than the level of what shocks.

\* \* \*

For most of the twentieth century, the dominant cultural texts in the English-speaking world — the ones most widely read, most widely discussed, most widely preserved and digitized and eventually fed into the training corpora of language models — encoded a remarkably consistent set of defaults. The scientist in the textbook was male. The nurse was female. The CEO in the business profile was male. The criminal in the news story was disproportionately Black. The romantic lead was straight. The family in the advertisement was white. The hero of the adventure story was a man. The person who needed saving was a woman.

These were not laws. They were not universal. There were exceptions, counterexamples, works that pushed deliberately against the defaults. But the statistical weight of the corpus — the sheer volume of text that encoded these patterns — meant that the patterns were real. And when researchers began to measure them, the numbers were striking.

The Geena Davis Institute on Gender in Media has tracked gender representation in film and television since 2004.⁷ Their analysis of family films found that for every one female character in a crowd scene, there were three male characters — a three to one ratio that audiences experienced as balanced, because three to one had become the baseline of what normal looked like. A scene with equal numbers of men and women was perceived by test audiences as female-dominated. The skew had become invisible. The default had become neutral.

The Annenberg Inclusion Initiative at USC has tracked representation in the top-grossing films annually since 2007.⁸ In their 2022 report, women represented thirty eight percent of speaking characters. Characters from underrepresented racial and ethnic groups remained underrepresented relative to the actual US population. LGBT characters remained rare. Characters with disabilities were largely absent.

\* \* \*

These numbers describe film and television. But film and television do not exist in isolation. They are accompanied by an enormous secondary ecosystem of text — reviews, criticism, profiles, interviews, think pieces, Wikipedia summaries, fan communities, cultural commentary, news coverage — all of which absorbed and reproduced the representational patterns of the primary content. All of this text — the vast secondary literature of cultural production — carried the representational defaults of its source material into the training data.

The model that trained on that corpus learned who doctors tend to be, who criminals tend to be, who heroes tend to be, who victims tend to be. Not from any explicit instruction. From the statistical weight of how those roles were filled in the text of a culture that distributed them unequally. The model's defaults are not its opinion. They are its education.

> The model's defaults are not its opinion. They are its education. And its education came from a culture that distributed roles unequally — which means the model, left to its own defaults, will reproduce that distribution as normal.

\* \* \*

Consider what this means practically. When you ask an AI to generate a story involving a surgeon and a nurse without specifying genders, the model's defaults will make a prediction. That prediction reflects the statistical distribution of how those roles were described in its training data — which reflects the statistical distribution of how those roles were filled and described in the culture that produced it. The model is not saying the surgeon should be male and the nurse should be female. It is saying that, in the text it learned from, those were the most common configurations. The default is a statistical description of the past, reproduced as a baseline for the present.

The practical consequence is that the model, operating at scale, becomes a vehicle for the reproduction of cultural defaults that many of the people using it have actively tried to move beyond. The person who has spent their career challenging the assumption that surgeons are male finds that the AI they are using to assist their work defaults to exactly the assumption they have been working against. The tool is not their enemy. It is their history. And their history, however much they have personally tried to change it, is what the model learned from.

---

## Section 8.5 — The Question to Carry

If this chapter has done its job, you are sitting with something uncomfortable. Not the comfortable discomfort of an abstract social problem that belongs to other people, other institutions, other choices made in other rooms. The specific discomfort of recognizing that the bias in the model came from the culture — and the culture includes you. The books you read. The television you watched. The news you absorbed. The language you used without examining it. The defaults you accepted without noticing they were defaults at all.

The model learned from all of it. From all of us. And it is reproducing what it learned with a fluency and a scale that has made something that was always present suddenly, inescapably visible.⁹

That visibility is worth sitting with before we move past it. Because the instinct, when confronted with systemic bias, is often one of two things. Either to locate the problem entirely in the system — the algorithm, the company, the data engineers — and absolve yourself of participation in it. Or to feel so implicated in something so large and so historical that the appropriate response seems to be paralysis or guilt rather than action. Both instincts are understandable. Neither is useful.

\* \* \*

The model's defaults are not destiny. They are starting points. Statistical averages derived from an unequal history, reproduced as baseline assumptions in a system that has no awareness it is making assumptions at all. They can be interrogated. They can be named. They can be explicitly overridden by anyone who knows to ask — and knowing to ask is precisely what this chapter has been building toward.

*Whose perspective is the default here?*

When the model generates a doctor, ask who it assumed the doctor was before you named them. When it generates a criminal, ask the same question. When it describes a neighborhood, a family, a leader, a victim, a scientist, a laborer — ask whose version of those things the model reached for first, and why, and what it left out in reaching for it. The question is not an accusation directed at the tool. It is an act of awareness directed at the output. It takes three seconds. It changes what you see.

\* \* \*

**Working With Bias in AI Outputs**

*Name What You Do Not Want Assumed:* The most direct intervention is the most effective one. If you are generating content involving people and the default matters to you, specify. Not as an afterthought — as part of the prompt. Tell the model the gender, the background, the role distribution you want represented. The model will follow explicit instruction more reliably than it will override its own statistical defaults. The default is what happens when you do not say anything. Say something.

*Ask What It Left Out:* After receiving any output involving people or groups, ask the model directly: who is not represented here? What perspective did this leave out? What would this look like from a different cultural or demographic starting point? A well-designed system will engage honestly with these questions. The answers will tell you more about the shape of the bias than the original output did — because the original output will not announce what it omitted. The omissions are invisible by definition. You have to go looking.

*Verify Against Reality:* When an AI output makes a claim — explicit or implicit — about what a group of people tends to do, look like, or be, check it against current data rather than accepting the model's statistical average from a historical corpus. The world is changing faster than the models can retrain. What was statistically typical in the text of 2010 may not be statistically typical now. The model does not know this. You do.

*Notice the Default Before You Override It:* The most valuable habit this chapter can offer is not a correction. It is attention. Before you accept any AI output that involves human beings — their roles, their qualities, their likely behaviors — notice who the default cast is. You may find it is exactly who you want. You may find it is not. You will not find anything at all if you do not look.

\* \* \*

The bias in the model is a reflection of the bias in the world that produced it. That world is not the past. It is the present, carrying the weight of the past in its language, its statistics, its defaults, its silences. The model did not introduce the bias. It magnified it.¹⁰ It made it reproducible at scale. It made it fast and fluent and authoritative and very, very hard to see.

Seeing it is the beginning. Not the end. Not the solution. The beginning.

What you do with what you see is the rest of the work. That work is yours. It always was.

---

*The Original Bug — Chapter 8: The Bias Mirror — Sandy B. Patterson*
