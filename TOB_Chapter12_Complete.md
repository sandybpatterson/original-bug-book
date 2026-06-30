# THE ORIGINAL BUG
### Chapter 12 — When Certainty Kills

---

## Section 12.1 — The Doctor Who Was Right

In the spring of 1847, a young Hungarian physician named Ignaz Semmelweis was working in the First Obstetrical Clinic of the Vienna General Hospital and watching women die. Not occasionally. Systematically. The ward he worked in had a mortality rate from childbed fever — puerperal fever, the infection that killed new mothers in the days after delivery — of around ten percent. In some months it climbed higher. The women knew. Pregnant women in Vienna begged not to be admitted to the First Clinic. Some delivered in the street rather than risk it. The reputation of the ward preceded Semmelweis everywhere he worked, a fact he found unbearable and could not explain.

Then, in the spring of that year, a close friend and colleague named Jakob Kolletschka died. Kolletschka was a pathologist. He had been accidentally cut by a student's scalpel during an autopsy and developed a systemic infection. When Semmelweis read the autopsy report, something broke open. The pathological findings in Kolletschka's body were identical — tissue by tissue, organ by organ — to the findings in women who had died of childbed fever. Kolletschka had died of something acquired during an autopsy. The women in the First Clinic were delivered by medical students and physicians who came directly from performing autopsies. The midwife-staffed Second Clinic, where the mortality rate was a fraction of the First's, had no such practice.

Semmelweis understood. Cadaverous particles — what we would now call pathogenic microorganisms — were being carried on the hands of the doctors and students from the autopsy room to the delivery ward. He instituted handwashing with a chlorinated lime solution. The mortality rate in the First Clinic dropped from around ten percent to around one percent within months.¹ He had the data. He had the intervention. He had the result.

The medical establishment rejected him.

\* \* \*

The rejection was not immediate and it was not universal. Some colleagues were interested. Some were persuaded. But the dominant response — from the most eminent physicians in Vienna and beyond, from the men whose certainty about how disease worked carried the weight of institutional authority — was dismissal. Sometimes polite. Sometimes contemptuous. Always certain.

The certainty had a foundation. It was called miasma theory — the prevailing medical framework of the era, which held that disease was caused by bad air, by atmospheric conditions, by the emanations of decaying organic matter. It was not a fringe belief. It was the established science of the time, endorsed by the most rigorous medical thinkers in Europe, supported by observations that seemed, within the framework, to confirm it. The framework was wrong in the specific way that matters most: it was wrong and certain of itself simultaneously, which meant that evidence that contradicted it could not register as evidence. It registered instead as an anomaly, an outlier, a finding that needed to be explained within the existing framework rather than a finding that challenged the framework itself.

Semmelweis's data was real. The mortality numbers were not ambiguous. The intervention produced a result that was, by the standards of any honest empirical assessment, dramatic and unambiguous. But the result could not be interpreted correctly by a mind already certain of a different explanation — because interpretation requires a framework, and the framework the medical establishment carried into the assessment of his data was a framework in which his explanation was impossible. Cadaverous particles on hands could not cause childbed fever, because childbed fever was caused by bad air. The data said otherwise. The certainty of the framework said otherwise more loudly.

> The framework was wrong and certain of itself simultaneously — which meant that evidence contradicting it could not register as evidence. It registered instead as an anomaly to be explained within the existing theory rather than a challenge to the theory itself.

\* \* \*

Semmelweis spent the next decade trying to be heard. He wrote letters. He published data. He grew increasingly desperate and, as the rejection continued, increasingly erratic in his advocacy — which gave his opponents grounds for dismissing him that had nothing to do with the evidence. He was eventually dismissed from his hospital position, returned to Budapest, and continued to practice and advocate there. In 1865 he was committed to a mental asylum. He died two weeks later, at the age of forty-seven, of an infection — almost certainly a sepsis of the kind he had spent his career trying to prevent, possibly contracted at the asylum itself.²

Germ theory was formally established within a decade of his death. Louis Pasteur and Robert Koch confirmed what Semmelweis had demonstrated empirically without the theoretical framework to explain it. The handwashing intervention he had instituted — and that had been abandoned after his dismissal — was reinstated and became foundational to medical practice worldwide. The women who died of childbed fever in European hospitals between 1847 and the wide acceptance of germ theory are not countable with precision. Estimates run into the hundreds of thousands.

They did not die because nobody had the answer. They died because the answer was held by someone the establishment was certain was wrong, in a field that was certain it was right, at a moment when certainty and evidence had come apart completely — and certainty had won.

\* \* \*

This chapter is not a history lesson about nineteenth-century medicine. It is a chapter about what certainty costs when the conditions are right — when the stakes are high enough, when the confident framework is wrong enough, when the correction mechanisms are absent or disabled. Semmelweis is the opening because his case makes the mechanism visible with a clarity that more recent examples, embedded in still-contested debates, cannot always achieve. The mechanism is simple and it is terrible: certainty, once achieved, filters the evidence that reaches it. Not through malice. Through architecture. The certain mind does not experience itself as filtering evidence. It experiences itself as evaluating evidence and finding it wanting. The filtering happens below the threshold of awareness, in the same motivated reasoning system that section 11.2 of this book documented — and in a high-stakes domain with no error-correction system in place, the filtering goes on until the consequences become impossible to ignore.

The question this chapter is going to sit with is what happens when that mechanism — the certain framework filtering the contradicting evidence, the correction arriving too late — is running not in one physician's mind in one hospital in Vienna, but in an AI system processing millions of cases simultaneously, trained on data shaped by the same overconfident human frameworks it is now amplifying back to the humans who consult it.

The stakes have not changed. The scale has.

---

## Section 12.2 — The Anatomy of Lethal Certainty

Overconfidence is everywhere. It runs in every human mind, shapes every human judgment, operates in every domain where people form beliefs and make predictions and reach conclusions. It is, as Chapter 3 of this book established, a structural property of human cognition — not a flaw in certain people under certain conditions but a feature of the architecture, built in by the evolutionary pressure that valued decisive action over accurate self-assessment. The world is full of overconfident beliefs. Most of them are harmless. Most of them correct themselves eventually through the ordinary friction of experience — the prediction fails, the plan does not work, the belief meets reality and loses.

What turns ordinary overconfidence into the thing described in this chapter is a specific combination of three conditions. They can occur independently. When they occur together, overconfidence stops being an epistemic inconvenience and becomes something with a body count. Understanding the three conditions is the prerequisite for understanding why the cases in the sections that follow are not cautionary tales from history but active, ongoing, structurally predictable features of the systems we are building and using right now.

\* \* \*

**Factor One — High Stakes**

The first condition is that the domain must matter. Overconfidence about which restaurant will be better, which route will be faster, which film will be more enjoyable — these errors resolve themselves with minimal cost. The restaurant disappoints. The route is slower. The film is dull. The certainty that produced the choice is slightly chastened by the outcome and life continues. The low-stakes domain is self-correcting in a way that makes overconfidence manageable.

High-stakes domains do not self-correct in the same way. Medicine, law, finance, engineering, public health, military decision-making — in these domains the gap between a confident wrong belief and its correction can be measured in lives, in liberty, in financial ruin, in the structural failure of systems that millions of people depend on. The overconfident diagnosis does not simply resolve into a milder condition after a week. The wrongful conviction does not correct itself when the real perpetrator commits another crime. High-stakes domains punish overconfidence at a magnitude that low-stakes domains do not — and they punish it after the point of correction has often already passed.

**Factor Two — Scale**

The second condition multiplies the first. A single overconfident physician practicing alone makes errors that affect the patients in their clinic. A medical diagnostic protocol, built on an overconfident framework and embedded in software used by thousands of physicians, makes errors that affect every patient in every clinic running that software. The overconfidence has not changed. The scale has. And scale does something to overconfidence that individual instances do not — it removes the ordinary corrective feedback that individual practitioners receive from their own error history.

A single physician who makes the same diagnostic error repeatedly will eventually notice the pattern — in their outcomes, in their mortality rates, in the cases that came back wrong. The individual error-correction mechanisms described in Chapter 11 have a chance to engage. A systemic protocol that makes the same error across thousands of practitioners simultaneously does not produce that individual corrective feedback. Each practitioner sees a small slice of the errors. No single practitioner sees enough of the pattern to recognize it as a pattern. The scale that makes the system powerful also makes the overconfidence it encodes invisible to the people running it.³

**Factor Three — Irreversibility**

The third condition is the one that converts error into catastrophe. Many high-stakes, large-scale errors can still be corrected if the correction mechanism is fast enough — if the error is detected before the consequences become permanent. The bridge that is built with a calculation error can be reinforced before it fails. The drug that produces unexpected side effects can be withdrawn before the side effects become widespread.

Irreversible errors cannot be corrected after the fact. The person who has died of a missed diagnosis. The years served by someone wrongfully convicted. The ecological damage from a policy implemented at scale before its consequences were understood. The lives lost while an established medical framework filtered out the evidence that would have prevented them. These errors happened. They cannot be made not to have happened.⁴ And the certainty that produced them — the overconfidence that filtered the contradicting evidence before it could register — is the specific cognitive failure that made the irreversibility possible, because it disabled the correction mechanism before the consequences arrived.

> Certainty disables the correction mechanism before the consequences arrive. By the time the error is visible, the irreversibility has already occurred. Certainty is not the cause of the harm in any simple sense. It is the removal of the last thing that could have prevented it.

\* \* \*

Semmelweis's Vienna had all three conditions. Medicine is high stakes. The Vienna General Hospital was one of the largest and most influential medical institutions in Europe — a center of training and research whose practices propagated outward to physicians across the continent. And the women who died of childbed fever while the argument continued were irreversibly dead. There was no correction that reached them.

The three conditions are not unusual. They are the normal operating environment of medicine, law, criminal justice, financial systems, public health, and infrastructure — the domains where society concentrates its most consequential decisions and where, not coincidentally, algorithmic systems are being most aggressively deployed. The AI systems entering these domains are not entering them as neutral tools that happen to be applied in high-stakes contexts. They are entering them as systems that encode the overconfidence of their training data, that operate at the scale that makes individual error-correction invisible, and that in some cases produce outputs that are acted on before the irreversibility of any particular error becomes clear.

---

## Section 12.3 — Certainty at Scale

The medical establishment that rejected Semmelweis was certain. It was also human-scale certain — certain in the minds of a defined number of influential physicians, operating in a defined number of institutions, whose certainty propagated through the mechanisms available to nineteenth-century medicine: journals, conferences, teaching hospitals, professional authority. The damage it caused was enormous. It was also, in historical terms, eventually correctable. The correction took decades and cost hundreds of thousands of lives. But it came. Germ theory arrived. The framework was replaced. The handwashing was reinstated.

The question this section is asking is what happens when that same certainty — the confident framework that filters contradicting evidence, the overconfident output that makes the human receiving it less likely to question than they would have been without it — is running inside a system that processes not dozens of cases per physician per year but millions of cases simultaneously, across thousands of institutions, at a speed that makes the error pattern invisible until long after the consequences have accumulated.

The answer is three cases. Each one documented. Each one different in domain and in the specific mechanism of amplification. Each one illustrating a version of the same fundamental dynamic: AI confidence making human overconfidence worse.

\* \* \*

**Case One — Medical Diagnosis — The Automation Bias Problem**

In 2018 a systematic review examined the performance of deep learning algorithms in medical image analysis — the AI systems being deployed to assist radiologists, pathologists, and dermatologists in identifying disease from scans, slides, and photographs. The headline finding received considerable positive attention: in several specific tasks, the algorithms matched or exceeded the diagnostic accuracy of specialist physicians.⁵

A quieter finding in the same body of research received considerably less attention. It concerned not the accuracy of the AI systems in isolation but what happened to human physician accuracy when the AI was present. The phenomenon has a name in human factors research: automation bias. It describes the well-documented tendency of human operators, when working alongside automated systems, to reduce their own independent evaluation and defer to the automated output — even when the automated output is wrong and the human, operating independently, would have caught the error.⁶

The AI diagnostic tool that matches a specialist's accuracy when the specialist is working independently does not necessarily improve overall system accuracy when deployed as an assistant. In some conditions it degrades it — because the confident AI output suppresses the physician's independent judgment in exactly the cases where that independent judgment would have caught what the AI missed. The physician who would have ordered a confirmatory test, who would have paused at an ambiguous finding, who would have noted something that did not quite fit — does not pause, does not order the test, does not note the anomaly when the AI has already produced a confident assessment. The AI's certainty borrows against the physician's uncertainty and spends it.

\* \* \*

**Case Two — Financial Systems — The Flash Crash**

On the afternoon of May 6, 2010, the United States stock market experienced one of the most dramatic and disorienting events in its history. In the space of approximately thirty-six minutes, the Dow Jones Industrial Average fell nearly a thousand points — at the time the largest intraday point decline in history — and then recovered most of the loss in the following twenty minutes. Individual stocks briefly traded at absurd prices: some fell to a penny, others rose to thousands of dollars above their previous value. The event became known as the Flash Crash.

The investigation that followed identified a complex cascade of causes.⁷ But at the center of the event was a specific dynamic that illuminates the chapter's argument precisely. Automated trading algorithms — systems operating at speeds no human trader can match, executing thousands of transactions per second based on pattern recognition in market data — had, under unusual conditions, entered a feedback loop with each other. Each system was reading the market signals produced partly by the other systems and trading on those signals, which produced further signals, which produced further trading. The certainty of each individual algorithm — the confident assessment that this pattern represented a buying or selling opportunity — was amplified by the certainty of every other algorithm reading the same degraded data. Human traders, watching the cascade on their screens, were effectively locked out of the correction. The speed of the automated certainty exceeded the speed of the human uncertainty that might have interrupted it.

The Flash Crash resolved because the automated systems eventually hit circuit breakers — pre-programmed limits that imposed a pause on trading — and human judgment had a chance to re-enter. The market recovered. No one died. But the event revealed, with unusual clarity, what happens when confident automated systems operating at machine speed amplify each other's overconfidence in a high-stakes, irreversible-at-the-moment-of-execution domain.

> The certainty of each individual algorithm was amplified by the certainty of every other algorithm reading the same degraded data. Human judgment was effectively locked out. The correction was a pause forced from outside the system — and without it, the cascade would have continued.

\* \* \*

**Case Three — Criminal Justice — The Confident Score**

COMPAS has appeared in this book before — in Chapter 4, in the context of heuristics, and in Chapter 8, in the context of bias. It returns here for a third time because the criminal justice context illustrates the irreversibility condition more starkly than any other domain this book examines. A risk score that contributes to a sentencing decision cannot be taken back after the sentence begins. The years served are not recoverable. The certainty of the algorithm — the confident numerical output that presents a human being's likelihood of reoffending as a precise score — does not hedge. It does not express calibrated uncertainty. It produces a number, and the number carries the authority of a system that processed hundreds of variables and arrived at a conclusion.

Research on judicial decision-making with algorithmic risk scores has found that judges given a risk score, even when explicitly told the score is imperfect and should be treated as one input among many, show significant anchoring effects — their final decisions cluster around the score in ways that suggest the number is doing more work than the instruction to treat it as one input would predict.⁸ The algorithm's certainty — expressed as a number, precise and quantitative and apparently objective — was more influential than the instruction to treat it with appropriate skepticism. The judge who would have weighed the full picture more independently, without the score, was anchored to the score by its confident presentation. The human overconfidence was not added to the algorithmic overconfidence. The algorithmic overconfidence replaced the human uncertainty that would otherwise have been present — and in doing so, removed the last buffer between a confident wrong number and an irreversible consequence.

\* \* \*

Three cases. Three domains. Three versions of the same mechanism: an AI system's confident output making the human receiving it more certain than they would have been without the AI, at the precise moment when less certainty was warranted. Not three AI systems that were dramatically wrong. Three AI systems that were confident in ways that suppressed the human doubt that would have caught what they missed.

Semmelweis's opponents were not stupid. They were certain. The physicians deferring to the diagnostic AI, the traders watching the algorithmic cascade, the judges anchoring to the risk score — none of them were stupid either. They were operating in environments that had handed them certainty more confident than the evidence warranted, and the human mind, as this book has been establishing across twelve chapters, does not naturally resist certainty when certainty is offered. It accepts it. It acts on it. It files the inconvenient uncertainty under: the system knows more than I do.

Sometimes the system does. That is what makes this hard.

And sometimes the system is certain about exactly the thing it should be uncertain about. That is what makes it dangerous.

---

## Section 12.4 — The Loop

What section 12.3 described was bad. What this section describes is worse. Section 12.3 was about a single interaction — overconfident AI output making an overconfident human more certain at a specific moment of decision. That is a static problem. Identifiable in principle. Correctable in principle, if you know to look for it and have the institutional structures to impose the looking.

What this section describes is dynamic. It is what happens when the interaction repeats — when the outcomes shaped by the overconfident human-AI interaction become the training data for the next generation of the AI, which learns from the contaminated outcomes and produces more confident outputs, which make the humans who receive them more certain, whose more certain decisions produce more contaminated outcomes, which go back into the training data. Round and round. Each iteration slightly more certain than the last. Each iteration with slightly less access to the correcting friction of genuine uncertainty. The feedback loop that tightens certainty until the system that was once overconfident has become, functionally, a machine for preventing its own correction.

\* \* \*

Consider what this looks like in medicine. A diagnostic AI is trained on a dataset of patient cases — symptoms, imaging, lab results, physician diagnoses, and outcomes. The physician diagnoses in the training data are not perfectly accurate. They reflect the overconfidence documented in Chapter 3, the anchoring bias documented in Chapter 4, the narrative constructions documented in Chapter 6. The model learns from these diagnoses. It encodes their systematic biases as patterns. It produces outputs that reflect those patterns — confidently, fluently, in the same direction the biased training data pointed.⁹

The model is deployed. Physicians use it. Automation bias, as documented in section 12.3, leads some physicians to defer to the model's confident outputs rather than exercising independent judgment. Their diagnoses — now shaped by the model's confident outputs — are recorded in the medical record. Patients are treated based on these diagnoses. Outcomes are observed. And those outcomes — the outcomes of diagnoses that were shaped in part by the previous model's overconfidence, filtered through the automation bias of the physicians who received its outputs — become part of the training data for the next generation of the model.

The next generation of the model learns from a dataset that has been subtly shifted in the direction of its predecessor's overconfidence. It produces outputs that are slightly more certain in the same direction. The physicians who receive those outputs defer slightly more. The diagnoses are slightly more skewed. The outcomes are slightly more contaminated. The training data for the subsequent generation is slightly more compromised. The loop has completed one iteration. It begins again.

> Each iteration is slightly more certain than the last. Each iteration with slightly less access to the correcting friction of genuine uncertainty. The feedback loop tightens until the system that was once merely overconfident has become, functionally, a machine for preventing its own correction.

\* \* \*

This is not a hypothetical. It has a name in the research literature on machine learning: model collapse — the phenomenon by which a model trained on data influenced by previous model outputs progressively diverges from the underlying reality it was intended to model.¹⁰ The research on this is relatively recent because the conditions that produce it — AI systems operating at sufficient scale and duration for the feedback effects to become measurable — are themselves relatively recent. But the phenomenon has been documented, its mechanisms are understood, and its implications for high-stakes domains where AI systems are both influencing outcomes and being retrained on those outcomes are the subject of growing concern among the researchers who study it most carefully.

The financial domain has seen versions of this for longer, because algorithmic trading systems have been operating at significant scale for more than two decades. When enough capital is being managed by systems that learned their strategies from historical market data, the systems themselves begin to move the market in ways that alter the data on which future systems will be trained.¹¹ The strategies that worked historically worked partly because the market had not yet been shaped by systems implementing those strategies. The model trained on pre-strategy data produces confident outputs in a market that no longer behaves the way the training data described. The confidence persists. The underlying reality has moved.

\* \* \*

There is a human version of this too. It has been running longer than any AI system. It is called institutional consensus — the process by which a field of knowledge, over time, becomes increasingly certain of its own framework, increasingly resistant to the evidence that challenges it, and increasingly likely to produce new practitioners who have been trained on the certain framework and therefore share its blind spots.

This is what Semmelweis encountered. The physicians who rejected his evidence were not individually certain in a vacuum. They were the products of a training system — medical education, clinical apprenticeship, the accumulated literature of the field — that had been encoding the certainty of miasma theory for generations. Each generation trained on the confident framework produced practitioners who were certain of the framework. The framework was not merely believed. It was reproduced, iteration by iteration, into the minds of every physician who encountered it, until it was so deeply embedded in the institutional structure of medicine that the handwashing of a single Hungarian physician could not dislodge it.

The difference between that process and the AI feedback loop described above is speed and scale. The human institutional consensus loop iterated across decades and trained thousands of practitioners. The AI feedback loop can iterate across months and influence the decisions of millions of people. The mechanism is the same. The velocity is not. And velocity, in a domain with irreversible consequences, is not a neutral variable.

\* \* \*

What breaks the loop?

Not better AI, on its own. A more accurate model, trained on the same contaminated data, will be more accurate in the direction the contaminated data pointed — which is not the same as being more accurate about the underlying reality. Not more cautious physicians, on their own. Individual caution cannot correct for a systemic bias that is invisible to the individuals encountering it, distributed across enough practitioners that no single one sees the pattern, and encoded in the confident outputs of a system that carries institutional authority.

What breaks the loop is the same thing that broke the miasma theory loop — external challenge. Evidence that arrives from outside the self-reinforcing system and cannot be accommodated within it. Researchers who examine the model's outputs against ground truth that does not come from the model's own training data. Red teams whose job is specifically to find what the confident system has missed. Audit requirements that force the documentation of error in a form that the motivated reasoning cannot silently release. The notebook, scaled to the institutional level — the external record that the loop cannot edit.

These are not comfortable interventions. They require building friction back into systems that have been optimized to remove it. They require treating uncertainty as an asset rather than a problem to be solved. They are also, given what the loop produces when it runs unchecked, the most important engineering and governance problem in the deployment of AI in high-stakes domains. The certainty is not the enemy. Certainty without correction is. And correction requires, above all else, the preservation of the genuine uncertainty the loop is designed to eliminate.

---

## Section 12.5 — The Value of Doubt

This chapter has been the darkest in the book. That was necessary. Not for the sake of alarm — alarm without direction is just anxiety with better sourcing — but because the cases documented here are real and the mechanism is real and the trajectory, without intervention, is not hypothetical. The feedback loop described in section 12.4 is not a future risk. It is a present condition. It is running now, in varying degrees, in the medical, financial, and criminal justice systems that the three cases of section 12.3 represent. Understanding it is not pessimism. It is the prerequisite for the only thing that actually helps.

What actually helps is not more confidence. It is not better AI, on its own. It is not more data, more processing power, more sophisticated models. All of those things are useful. None of them address the fundamental problem, which is not the quantity or quality of the information available to the system but the certainty with which the system's outputs are delivered and received. The fundamental problem is the removal of doubt from a domain where doubt is the only reliable early warning system for the kind of errors that cannot be corrected after they have been made.

> The value of doubt is not philosophical. It is structural. Doubt is the pause between the confident output and the irreversible action. It is the physician who orders the confirmatory test. It is the last buffer between a confident wrong answer and a consequence that cannot be taken back.

\* \* \*

Tetlock's superforecasters, introduced in Chapter 3, did not outperform their peers by being right more often in any simple sense. They outperformed them by treating their own certainty as a variable — by attaching probabilities to beliefs and then actively looking for reasons those probabilities should be revised. They were comfortable with doubt in the specific, disciplined sense of holding a belief provisionally and remaining genuinely open to the evidence that would warrant changing it. That comfort was not passivity. It was the most active thing they did. It required more effort, not less, than simply being certain.

The superforecasters were operating as individuals, forecasting political events, with no AI system amplifying their conclusions or feeding their outputs back into the data their successors would be trained on. The challenge of institutional doubt — of building the superforecaster's relationship with uncertainty into the culture and governance of large-scale AI deployments in high-stakes domains — is considerably harder. But the principle is identical. Uncertainty is not weakness. It is the system's immune response. Remove it, and the system loses the ability to detect and correct the errors that will otherwise accumulate until they are no longer correctable.

\* \* \*

What does this mean for you, reading this, using the tools this book has been examining throughout? It means something specific and immediately applicable.

When a confident system — human or machine — tells you something in a high-stakes domain, the most important question you can ask is not whether the output is right. It is whether the system has been designed to catch it when it is wrong. Whether there is a feedback mechanism that preserves genuine uncertainty rather than optimizing it away. Whether the confident output you are receiving is the product of a loop that has been checking its own certainty against external reality, or the product of a loop that has been reinforcing its own certainty against itself.

You cannot always answer that question. The systems are often not transparent enough for an individual to audit their feedback architecture from the outside. But you can always ask it. And asking it — out loud, to the person or institution presenting the confident output — is itself a form of the external challenge that breaks the loop. The physician who is asked by their patient whether the diagnostic AI's recommendation has been validated against cases like theirs. The judge who is required to document the reasoning that led them to weigh the risk score the way they did. The financial institution whose algorithm is required to demonstrate that its confidence intervals were accurate over the relevant time period. These are uncomfortable requests. They impose friction on systems that have been optimized for smooth, confident, efficient output. That friction is not a bug. It is the point.

\* \* \*

Semmelweis died of the thing he had figured out how to prevent. That is the sharpest possible statement of what it costs when the correction is right and the certainty of the established system is wrong and the two cannot be reconciled before the consequences become permanent. It is also, if you hold it in mind long enough, something more than a cautionary tale. It is a description of the stakes of the problem this book has been examining from the beginning — the problem of a species that built its cognitive shortcuts into every system it created, that encoded its overconfidence into every institution it established, and that is now building those same shortcuts and that same overconfidence into machines that operate at a scale and speed that make the human versions look modest.

The correction is available. It was available to Semmelweis and the medical establishment of 1847 — the data was there, the intervention was there, the mortality statistics were there — and they could not use it because the certainty of the existing framework had disabled the correction mechanism before the correction arrived. The correction is available now. The research is there. The documented cases are there. The feedback loop mechanism is understood. What remains is whether the institutions building and deploying these systems will build the correction mechanisms before the consequences make them necessary.

And what remains for you — the person using these systems, consulting them, making decisions with their assistance — is the practice of asking the one question that certainty, by its nature, does not ask itself.

*What if this is wrong?*

Not to paralyze. Not to refuse the output. To hold the space open, for one moment before the action, for the possibility that the confident system has been certain about exactly the thing it should be uncertain about. To be the pause in the loop. To be the thing the feedback loop is always, by design, trying to eliminate.

To be, in whatever small way is available to you in the moment, the friction that saves the thing that would otherwise be lost.

---

*The Original Bug — Chapter 12: When Certainty Kills — Sandy B. Patterson*
